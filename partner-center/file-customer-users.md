---
title: Champs du fichier. csv pour importer plusieurs utilisateurs pour un compte client
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pour ajouter plusieurs utilisateurs à un compte client, créez un fichier de valeurs séparées par des virgules (. csv) avec les champs appropriés.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150979"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Ajouter plusieurs utilisateurs à un compte client en créant un fichier. csv

**Rôles appropriés** : administrateur général

Ajoutez simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires. Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.

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
| Nom complet    | Nom affiché dans l’espace partenaires (champ obligatoire)                            | limité à 50 caractères                         |
| Courrier   | Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)           | Chaque utilisateur doit avoir une adresse e-mail unique |
| Mise à jour de l'état   | Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé avec succès | \*\*Conserver vide\*\*                        |

## <a name="next-steps"></a>Étapes suivantes

- [Guide pratique pour ajouter plusieurs utilisateurs pour un client](adding-multiple-users-to-a-customer-account.md)