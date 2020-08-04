---
title: Ajouter plusieurs utilisateurs pour un compte client
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pour ajouter plusieurs utilisateurs au compte d’un client, téléchargez un fichier de données dans l’espace partenaires à l’aide du format de fichier de valeurs séparées par des virgules (. csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535739"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Charger un fichier. csv d’utilisateurs sur le compte d’un client


**S’applique à**

- Espace partenaires

**Rôles appropriés**

- Administrateur général

Ajoutez simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Créer le fichier des utilisateurs du client et le télécharger vers le compte client

1. Créez un fichier de données CSV avec les données décrites ci-dessus. Enregistrez le fichier pour pouvoir le retrouver ultérieurement. Consultez [champs pour le fichier. csv pour importer plusieurs utilisateurs pour un compte client](file-customer-users.md). 

2. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

3. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

4. Sélectionnez l’onglet **utilisateurs et licences** du client, puis cliquez sur **Télécharger les utilisateurs**.

5. Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.

6. Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.

7. Sélectionnez **Valider**.

    **Remarque**    La plupart des erreurs de création de compte sont provoquées par des problèmes de fichiers de données, notamment des informations manquantes, des adresses de messagerie incorrectes ou en double ou des enregistrements trop nombreux dans le fichier.

8. Une fois que l’espace partenaires a validé le fichier, sélectionnez l' **emplacement** géographique pour les nouveaux utilisateurs.
9. Sélectionnez **Enregistrer**.
10. Chargez les informations sur le mot de passe temporaire pour les utilisateurs.

    >[!IMPORTANT]
    > Veillez à télécharger le fichier avec les mots de passe temporaires maintenant, car vous ne pourrez pas le faire par la suite. Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.

11. Les autorisations qui sont attribuées automatiquement aux nouveaux utilisateurs **peuvent utiliser des licences et des services** . 

## <a name="next-steps"></a>Étapes suivantes

- [Autoriser les clients dans l’espace partenaires à acheter leurs propres produits ou services](give-customers-permission.md)
