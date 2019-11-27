---
title: Créer plusieurs utilisateurs pour un compte client | Espace partenaires
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: chargement groupé, ajouter plusieurs utilisateurs à un compte client, ajouter des utilisateurs du client, chargement groupé des utilisateurs du client, compte client, utilisateurs du client, utilisateurs
ms.localizationpriority: medium
ms.openlocfilehash: 5c9de7ed78a0494790b447d1755d5eef70a89cca
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253177"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Ajouter plusieurs utilisateurs à un compte client

**S’applique à**

-  Espace partenaires

Vous pouvez ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires. Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.

## <a href="" id="creatingtheimportcsvfile"></a>Exigences relatives aux fichiers de données


Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :

-   Vous devez posséder des autorisations d’administrateur global sur le compte client.
-   Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.
-   Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois. Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.
-   Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.
-   N’entrez que les données décrites ci-dessous. Les autres données bloqueront le chargement.

Entrez les données suivantes dans le fichier de données&nbsp;:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nom de la colonne** | **Description**                                                              | **Contrainte**                             |
| Prénom      | Prénom de l’utilisateur (champ facultatif)                                           | 50&nbsp;caractères maximum                         |
| Nom       | Nom de l’utilisateur (champ facultatif)                                            | 50&nbsp;caractères maximum                         |
| Display name    | Nom affiché dans l’espace partenaires (champ obligatoire)                            | 50&nbsp;caractères maximum                         |
| E-mail           | Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)           | Chaque utilisateur doit avoir une adresse de messagerie unique. |
| Mise à jour de l’état   | Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé | \*\*laissez un\*vide \*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Pour créer plusieurs comptes d’utilisateur

<a href="" id="creatingtheaccounts"></a>
1.  Créez un fichier de données CSV avec les données décrites ci-dessus. Enregistrez le fichier pour pouvoir le retrouver ultérieurement.
2.  Dans le menu **espace partenaires** , sélectionnez **clients**, puis choisissez un client dans la liste.
3.  Sélectionnez **Charger des utilisateurs**.
4.  Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.
5.  Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.
6.  Sélectionnez **Valider**.

    **Notez**  la plupart des erreurs de création de compte sont provoquées par des problèmes de fichiers de données, notamment des informations manquantes, des adresses de messagerie incorrectes ou en double ou des enregistrements trop nombreux dans le fichier.

7.  Une fois que l’espace partenaires a validé le fichier, sélectionnez l' **emplacement** géographique pour les nouveaux utilisateurs.
8.  Sélectionnez **Enregistrer**.
9.  Téléchargez le mot de passe temporaire des utilisateurs.

**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après. Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.

10. Les autorisations **Peut utiliser les licences et services** sont automatiquement attribuées aux nouveaux utilisateurs. 

 

 



