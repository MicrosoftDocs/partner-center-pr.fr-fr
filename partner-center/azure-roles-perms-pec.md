---
title: Rôles, autorisations pour le crédit gagné par le partenaire
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En savoir plus sur les rôles et les autorisations que les partenaires peuvent obtenir en tant que crédit gagné (PEC). Ils diffèrent des rôles à travailler dans l’espace partenaires.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fa6241755e228e36abdd15022c127d2b243b488f
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390586"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Rôles et autorisations admissibles pour obtenir un crédit gagné par le partenaire

Les rôles suivants correspondent aux niveaux d’autorisation qui déterminent si un partenaire est éligible pour les crédits acquis par le partenaire.

>[!Important]
>Ces rôles et autorisations ne sont pas les mêmes que les rôles et les autorisations dont un utilisateur a besoin pour travailler dans l’espace partenaires.

|**Rôle**   |**Description**   |**PEC éligible**   |
|-----------------|:------------------|:--------------|
|Propriétaire  |Vous gérez tout, y compris l’accès aux ressources.|Oui|
|Contributeur |Vous gérez tout sauf en accordant l’accès aux ressources.|Oui|
|Lecteur|Vous pouvez tout afficher, mais ne pas apporter de modifications|Non|
|ACRDelete|acr delete|Oui|
|ACRImageSigner|signataire d’image ACR|Oui|
|ACRPull|tirer (pull) acr|Oui|
|AcrPush|envoyer (push) acr|Oui|
|AcrQuarantineReader|lecteur de données de quarantaine ACR|Non|
|AcrQuarantineWriter| écriture de données de quarantaine ACR|Oui|
|Contributeur du service de gestion des API|Peut gérer le service et les API|Oui|
|Rôle d’opérateur du service Gestion des API|Peut gérer le service, mais pas les API|Oui|
|Rôle de lecteur du service Gestion des API|Accès en lecture seule au service et aux API|Non|
|Contributeur de composants Application Insights|Gère les composants de Application Insights|Oui|
|Débogueur de capture instantanée d’Application Insights|Autorise l’utilisateur à consulter et à télécharger les instantanés de débogage collectés à l’aide du débogueur de capture instantanée Application Insights. Ces autorisations ne sont pas incluses dans les rôles Propriétaire et Contributeur.|Oui|
|