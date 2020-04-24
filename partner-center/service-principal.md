---
title: Principal de service Azure AD | Espace partenaires
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ajouter un principal de service à votre locataire Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, plan Azure, principal de service, application Azure AD
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2020
ms.locfileid: "75716890"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Ajouter une application Azure AD (principal de service) dans l’Espace partenaires

Dans le programme Place de marché commerciale de l’Espace partenaires, vous pouvez désormais ajouter une application Azure AD (principal de service) en tant qu’utilisateur dans votre compte Espace partenaires. (Avant, vous pouviez le faire dans votre compte Portail Cloud Partner, mais maintenant que vous avez migré vers l’Espace partenaires, ce compte est en lecture seule.) Notez que principal de service et application Azure AD sont synonymes.

## <a name="add-an-azure-ad-application-service-principal"></a>Ajouter une application Azure AD (principal de service)

1. Dans le tableau de bord de l’Espace partenaires, sélectionnez **Paramètres**, puis **Paramètres de développeur**.

2. Sélectionnez **Utilisateurs**, puis **Ajouter des applications Azure AD**.

3. Sélectionnez une application Azure AD existante ou créez-en une.

4. Si vous créez une nouvelle application Azure AD, incluez les informations suivantes :  

  


**URL de réponse** : URL avec laquelle les utilisateurs peuvent se connecter pour utiliser votre application Azure AD. 

**URI d’ID d’application** : Il s’agit d’un identificateur logique pour l’application Azure AD qui est présenté lors de l’envoi d’une demande d’authentification unique à Azure AD. 

**Rôles de sécurité** : Les rôles **Responsable** (identique au rôle « Propriétaire » dans le Portail Cloud Partner) et **Développeur** (identique au rôle « Contributeur » dans le Portail Cloud Partner) s’appliquent au programme Place de marché commerciale dans l’Espace partenaires et peuvent être associés à cette application Azure AD.  

  
