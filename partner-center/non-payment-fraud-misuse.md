---
title: Gestion des défauts de paiement, des fraudes ou des mauvaises utilisations
description: Découvrez les différents risques impliqués dans les transactions en ligne et les meilleures pratiques pour gérer et atténuer ces risques dans l’espace partenaires.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686294"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Gestion des défauts de paiement, des fraudes ou des utilisations abusives dans l’Espace partenaires

**S’applique à**

- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Administrateur général
- Administrateur de la gestion des utilisateurs
- Agent d’administration
- Administrateur de la facturation

Vous êtes financièrement responsable des achats frauduleux de vos clients et/ou du non-paiement des services achetés par les clients. Par conséquent, *nous vous recommandons vivement de mettre en place les contrôles d’atténuation des risques de prévention et de détection des fraudes*.

Pour éviter et/ou résoudre les problèmes d’activité ou de mauvaise utilisation frauduleuses, il est important de comprendre les risques potentiels et de développer des stratégies et des pratiques qui peuvent réduire votre exposition.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Application de la stratégie d’utilisation acceptable de Microsoft

Si Microsoft détecte une activité de partenaire ou de client que nous confirmons ou soupçonnons de violer la stratégie d’utilisation acceptable, nous allons prendre des mesures d’application. Le client peut être immédiatement suspendu. Vous serez averti des actions de mise en œuvre ou mises à jour sur vos demandes par Microsoft.

## <a name="abuse-of-service-risks"></a>Abus des risques de service

L' **abus des risques de service** signifie que les clients utilisent des services Cloud en violation de la stratégie d’utilisation acceptable de Microsoft.

### <a name="examples-of-abuse-of-service"></a>Exemples d’abus de service

Voici quelques exemples de violations de la stratégie d’utilisation acceptable de Microsoft :

- Courriers indésirables
- Piratage
- Attaques par déni de service distribué (DDoS)
- Exploration de données Bitcoin
- Distribution de logiciels malveillants
- Revente d’abonnements piratés

## <a name="theft-of-service-risks"></a>Vol de risques de service

Le **vol de risques de service** signifie que les clients n’ont pas l’intention de payer des services consommés. Ce vol peut impliquer l’utilisation de moyens de paiement volés, le fait de fournir des informations de facturation erronées et/ou la valeur par défaut des soldes en suspens.

### <a name="examples-of-service-theft"></a>Exemples de vol de service

Voici quelques exemples de ces risques de transactions en ligne :

- Transactions qui ne se produisent pas en personne (transactions de « carte de crédit absentes »)
- Identités déreprésentéees
- Services approvisionnés et utilisés avant la réception du paiement initial
- Marchés émergents et/ou régions à risque élevé pour la fraude en ligne
- Automatiser la création et l’achat de comptes par des acteurs incorrects

## <a name="managing-online-risk"></a>Gestion des risques en ligne

Vous pouvez utiliser les recommandations suivantes pour vous aider à développer des stratégies et des pratiques pour réduire votre exposition aux risques de transactions en ligne dans le cycle de vie de vos relations client.

### <a name="onboarding-new-customers"></a>Intégration de nouveaux clients

Les suggestions pour réduire les risques en ligne lors de l’intégration de nouveaux clients sont les suivantes :

- Établissez des relations personnelles avec les clients lorsque cela est possible (par exemple, en contactant les clients par téléphone).
- Vérifiez les informations d’identification et l’arrière-plan des clients via de meilleures méthodes (par exemple, en utilisant des bureaux de crédit ou des agences de rapports commerciaux commerciaux).
- Utilisez Multi-Factor Authentication (par exemple, la vérification SMS) lors de l’inscription pour réduire l’exposition à la création et à l’achat d’un compte robotique.
- Gérez et suivez les identités à l’aide de services (tels que les services d’identité numérique).
- Évaluez la force financière du client par le biais de systèmes de détection des fraudes de carte de crédit rigoureux.
- Établissez une stratégie effacer les regroupements. Détaillez votre processus de collecte et lorsque l’accès aux abonnements sera affecté par un non-paiement. (Vous pouvez désactiver l’accès ou [suspendre les abonnements d’un client](create-a-new-subscription.md#suspend-a-subscription) en cas de non-paiement.)

### <a name="managing-customer-accounts"></a>Gestion des comptes client

Les suggestions relatives à la gestion des comptes clients après achat sont les suivantes :

- Implémentez un processus pour recevoir, examiner, agir et répondre rapidement aux notifications Microsoft.
- Collaborez avec les clients pour comprendre leurs besoins en matière d’utilisation du Cloud, tout en définissant les seuils d’analyse appropriés. (Par exemple, vous pouvez [définir un budget de dépenses Azure mensuel](set-an-azure-spending-budget-for-your-customers.md) dans l’espace partenaires. Cette compréhension vous permet de surveiller l’utilisation des clients pendant le mois et de recevoir une notification lorsque les clients sont proches de leur budget.)
- Surveillez régulièrement les [journaux d’activité des clients](activity-logs.md) pour faciliter la détection des fraudes.
- Effectuez une action rapide lorsque des activités suspectes sont détectées.
- Évitez de fournir aux clients un accès administratif complet aux abonnements sans implémenter au préalable les contrôles d’atténuation des risques.

### <a name="managing-customer-billing"></a>Gestion de la facturation client

Les suggestions relatives à la gestion de la facturation cliente après achat sont les suivantes :

- Demander des prépaiements avant les transactions initiales et la facturation.
- N’acceptez pas les instruments de paiement à haut risque (tels que les cartes prépayées ou les cartes de valeur stockées).
- Surveillez les paiements des clients et les comptes chrono. Appliquez de manière agressive des processus rappels standardisés pour des paiements tardifs ou un non-paiement.

Pour plus d’informations sur les stratégies de réduction des risques en ligne, consultez le Guide de gestion des risques pour les [transactions en ligne.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
