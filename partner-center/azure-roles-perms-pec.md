---
title: Rôles, autorisations pour le crédit gagné par le partenaire
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En savoir plus sur les rôles et les autorisations que les partenaires peuvent obtenir en tant que crédit gagné (PEC). Ils diffèrent des rôles à travailler dans l’espace partenaires.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f84f1998258b0187537bac61edba9c6465aeb8e
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2020
ms.locfileid: "84908977"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Rôles et autorisations admissibles pour obtenir un crédit gagné par le partenaire

Les rôles suivants correspondent aux niveaux d’autorisation qui déterminent si un partenaire est éligible pour les crédits acquis par le partenaire.

>[!Important]
>Ces rôles et autorisations ne sont pas les mêmes que les rôles et les autorisations dont un utilisateur a besoin pour travailler dans l’espace partenaires.

|**Rôle**   |**Description**   |**PEC éligible**   |
|-----------------|:------------------|:--------------|
|Propriétaire  |Vous gérez tout, y compris l’accès aux ressources.|Yes|
|Contributeur |Vous gérez tout sauf en accordant l’accès aux ressources.|Yes|
|Lecteur|Vous pouvez tout afficher, mais ne pas apporter de modifications|No|
|ACRDelete|acr delete|Yes|
|ACRImageSigner|signataire d’image ACR|Yes|
|ACRPull|tirer (pull) acr|Yes|
|AcrPush|envoyer (push) acr|Yes|
|AcrQuarantineReader|lecteur de données de quarantaine ACR|No|
|AcrQuarantineWriter| écriture de données de quarantaine ACR|Yes|
|Contributeur du service de gestion des API|Peut gérer le service et les API|Yes|
|Rôle d’opérateur du service Gestion des API|Peut gérer le service, mais pas les API|Yes|
|Rôle de lecteur du service Gestion des API|Accès en lecture seule au service et aux API|No|
|Contributeur de composants Application Insights|Gère les composants de Application Insights|Yes|
|Débogueur de capture instantanée d’Application Insights|Autorise l’utilisateur à consulter et à télécharger les instantanés de débogage collectés à l’aide du débogueur de capture instantanée Application Insights. Ces autorisations ne sont pas incluses dans les rôles Propriétaire et Contributeur.|Oui|
|