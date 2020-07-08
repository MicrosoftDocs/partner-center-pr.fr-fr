---
title: Principal de service Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter un principal de service à votre locataire Azure AD. Cela revient à ajouter une application Azure AD (principal de service) dans l’Espace partenaires.
author: dhirajgandhi
ms.author: dhgandhi
Keywords: Azure, plan Azure, principal de service, application Azure AD
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: bd2880f57d1ccb3c3675fef4fae7499f7ac02f4b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949627"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Ajouter une application Azure AD (principal de service) dans l’Espace partenaires

Dans le programme Place de marché commerciale de l’Espace partenaires, vous pouvez désormais ajouter une application Azure AD (principal de service) en tant qu’utilisateur dans votre compte Espace partenaires. (Vous pouviez le faire précédemment dans votre compte Portail Cloud Partner ou CPP. Maintenant que vous avez effectué la migration vers l’Espace partenaires, le compte CPP est en lecture seule.)
 
>[!Note] 
>Principal du service et application Azure AD sont synonymes.

## <a name="add-an-azure-ad-application-service-principal"></a>Ajouter une application Azure AD (principal de service)

1. Dans le tableau de bord de l’Espace partenaires, sélectionnez **Paramètres**, puis **Paramètres de développeur**.

2. Sélectionnez **Utilisateurs**, puis **Ajouter des applications Azure AD**.

3. Sélectionnez une application Azure AD existante ou créez-en une.

4. Si vous créez une nouvelle application Azure AD, incluez les informations suivantes :  

   - **URL de réponse** : URL avec laquelle les utilisateurs peuvent se connecter pour utiliser votre application Azure AD.

   - **URI d’ID d’application** : identificateur logique pour l’application Azure AD qui est présenté lors de l’envoi d’une demande d’authentification unique à Azure AD.

   - **Rôles de sécurité** : Les rôles **Responsable** (identique au rôle « Propriétaire » dans le Portail Cloud Partner) et **Développeur** (identique au rôle « Contributeur » dans le Portail Cloud Partner) s’appliquent au programme Place de marché commerciale dans l’Espace partenaires et peuvent être associés à cette application Azure AD.  
