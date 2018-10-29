---
title: Créer plusieurs utilisateurs pour un compte client | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Vous pouvez ajouter plusieurs utilisateurs en même temps au compte d’un client, en chargeant un fichier de donnéesCSV dans l’Espace partenaires.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: chargement groupé, ajouter plusieurs utilisateurs à un compte client, ajouter des utilisateurs du client, chargement groupé des utilisateurs du client, compte client, utilisateurs du client, utilisateurs
ms.localizationpriority: medium
ms.openlocfilehash: 12bb42d4e1dcf5003ac8790be777c483f216fd6f
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795672"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Ajouter plusieurs utilisateurs à un compte client

**S'applique à**

-  Espace partenaires

Vous pouvez ajouter plusieurs utilisateurs à un compte client tous à la fois, en chargeant un fichier de données dans le format de fichier de valeurs séparées par des virgules (.csv) dans l’espace partenaires. Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis l’adapter à votre utilisation, ou vous pouvez créer un fichier de données à l’aide du modèle de données défini ci-dessous.

## <a href="" id="creatingtheimportcsvfile"></a>Conditions requises pour les fichiers de données


Pour ajouter plusieurs utilisateurs au compte d’un client par chargement groupé, vous devez respecter les conditions suivantes&nbsp;:

-   Vous devez posséder des autorisations d’administrateur global sur le compte client.
-   Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.
-   Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois. Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.
-   Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.
-   N’entrez que les données décrites ci-dessous. Les autres données bloqueront le chargement.

Entrez les données suivantes dans le fichier de données&nbsp;:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nom de la colonne** | **Description**                                                              | **Limitation**                             |
| Prénom      | Prénom de l’utilisateur (champ facultatif)                                           | 50&nbsp;caractères maximum                         |
| Nom       | Nom de l’utilisateur (champ facultatif)                                            | 50&nbsp;caractères maximum                         |
| Nom d’affichage    | Nom affiché dans l’espace partenaires (champ obligatoire)                            | 50&nbsp;caractères maximum                         |
| Email           | Adresse de messagerie professionnelle de l’utilisateur chez le client (champ obligatoire)           | Chaque utilisateur doit avoir une adresse de messagerie unique. |
| Mise à jour de l’état   | Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé. | \*\*Laisser vide\* \ *                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Pour créer plusieurs comptes d’utilisateur&nbsp;:

<a href="" id="creatingtheaccounts"></a>
1.  Créez un fichier de données&nbsp;CSV avec les données décrites ci-dessus. Enregistrez le fichier pour pouvoir le retrouver ultérieurement.
2.  Dans le menu **Espace partenaires** , sélectionnez **clients**, puis choisissez un client dans la liste.
3.  Sélectionnez **Charger des utilisateurs**.
4.  Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.
5.  Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.
6.  Sélectionnez **Valider**.

    **Remarque**la plupart des erreurs de création de compte sont provoquées par des problèmes de fichier de données, y compris les informations manquantes, des adresses de messagerie incorrectes ou dupliquées ou un trop grand nombre d’enregistrements dans le fichier.

7.  Lorsque l’espace partenaires a validé le fichier, sélectionnez l' **emplacement** géographique des nouveaux utilisateurs.
8.  Sélectionnez **Enregistrer**.
9.  Téléchargez le mot de passe temporaire des utilisateurs.

**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après. Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.

10. Nouveaux utilisateurs reçoivent automatiquement les autorisations de **peut utiliser les licences et services** . 

 

 



