---
title: Créer plusieurs utilisateurs pour un compte client | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Vous pouvez ajouter plusieurs utilisateurs en même temps au compte d’un client, en chargeant un fichier de données CSV dans l’Espace partenaires.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: chargement groupé, ajouter plusieurs utilisateurs à un compte client, ajouter des utilisateurs du client, chargement groupé des utilisateurs du client, compte client, utilisateurs du client, utilisateurs
ms.localizationpriority: medium
ms.openlocfilehash: 12bb42d4e1dcf5003ac8790be777c483f216fd6f
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584242"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Ajouter plusieurs utilisateurs à un compte client

**S’applique à**

-  Espace partenaires

Vous pouvez ajouter plusieurs utilisateurs à un compte client tout en même temps, en chargeant un fichier de données dans le format de fichier de valeurs séparées par des virgules (.csv) dans l’espace partenaires. Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires et puis de le modifier pour votre usage, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.

## <a href="" id="creatingtheimportcsvfile"></a>Exigences de fichier de données


Pour ajouter plusieurs utilisateurs au compte d’un client par chargement groupé, vous devez respecter les conditions suivantes&nbsp;:

-   Vous devez posséder des autorisations d’administrateur global sur le compte client.
-   Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.
-   Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois. Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.
-   Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.
-   N’entrez que les données décrites ci-dessous. Les autres données bloqueront le chargement.

Entrez les données suivantes dans le fichier de données&nbsp;:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nom de colonne** | **Description**                                                              | **Limitation**                             |
| Prénom      | Prénom de l’utilisateur (champ facultatif)                                           | 50&nbsp;caractères maximum                         |
| Nom       | Nom de l’utilisateur (champ facultatif)                                            | 50&nbsp;caractères maximum                         |
| Nom d’affichage    | Nom affiché dans l’espace partenaires (champ obligatoire)                            | 50&nbsp;caractères maximum                         |
| E-mail           | Adresse de messagerie professionnelle de l’utilisateur chez le client (champ obligatoire)           | Chaque utilisateur doit avoir une adresse de messagerie unique. |
| Mise à jour de l’état   | Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé | \*\*Laissez vide\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Pour créer plusieurs comptes d’utilisateur

<a href="" id="creatingtheaccounts"></a>
1.  Créez un fichier de données CSV avec les données décrites ci-dessus. Enregistrez le fichier pour pouvoir le retrouver ultérieurement.
2.  À partir de la **partenaires** menu, sélectionnez **clients**, puis choisissez un client dans la liste.
3.  Sélectionnez **Charger des utilisateurs**.
4.  Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.
5.  Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.
6.  Sélectionnez **Valider**.

    **Remarque**  la plupart des erreurs de création de compte sont dus à des problèmes de fichier de données, y compris les informations, les adresses de messagerie incorrect ou en double ou trop grand nombre d’enregistrements dans le fichier manquant.

7.  Une fois l’espace partenaires valide le fichier, sélectionnez le géographique **emplacement** pour les nouveaux utilisateurs.
8.  Sélectionnez **Enregistrer**.
9.  Téléchargez le mot de passe temporaire des utilisateurs.

**IMPORTANT :** Veillez à télécharger le fichier avec les mots de passe temporaires maintenant, car vous ne pourrez le faire ultérieurement. Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.

10. Les autorisations **Peut utiliser les licences et services** sont automatiquement attribuées aux nouveaux utilisateurs. 

 

 



