---
title: Ajouter plusieurs utilisateurs pour un compte client
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter simultanément plusieurs utilisateurs au compte d’un client. Téléchargez un fichier de données dans l’espace partenaires à l’aide du format de fichier de valeurs séparées par des virgules (. csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a9a94ac9d9022b33c7f909a258b66daa4312ad13
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436308"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a>Ajouter plusieurs utilisateurs à un compte client-charger un fichier de données dans l’espace partenaires

**S’applique à**

- Espace partenaires

**Rôles appropriés**

- Administrateur général

Vous pouvez ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires. Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Conditions requises pour les fichiers de données

Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :

- Vous devez posséder des autorisations d’administrateur global sur le compte client.
- Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.
- Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois. Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.
- Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.
- N’entrez que les données décrites ci-dessous. Les autres données bloqueront le chargement.

Entrez les données suivantes dans le fichier de données&nbsp;:

| **Nom de la colonne** | **Description**  | **Limite**  |
|:-------- |:------  |:----- |
| Prénom  | Prénom de l’utilisateur (champ facultatif)  | limité à 50 caractères  |
| Nom  | Nom de l’utilisateur (champ facultatif)  | limité à 50 caractères  |
| Nom d’affichage    | Nom affiché dans l’espace partenaires (champ obligatoire)                            | limité à 50 caractères                         |
| E-mail   | Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)           | Chaque utilisateur doit avoir une adresse e-mail unique |
| Mise à jour de l'état   | Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé | \*\*Conserver vide\*\*                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a>Pour créer plusieurs comptes d’utilisateur

<a href="" id="creatingtheaccounts"></a>

1. Créez un fichier de données CSV avec les données décrites ci-dessus. Enregistrez le fichier pour pouvoir le retrouver ultérieurement.

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

**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après. Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.

10. Les autorisations qui sont attribuées automatiquement aux nouveaux utilisateurs **peuvent utiliser des licences et des services** . 

 

 



