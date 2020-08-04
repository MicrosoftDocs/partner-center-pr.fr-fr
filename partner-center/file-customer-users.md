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
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528179"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="e1126-103">Ajouter plusieurs utilisateurs à un compte client en créant un fichier. csv</span><span class="sxs-lookup"><span data-stu-id="e1126-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="e1126-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="e1126-104">**Applies to**</span></span>

- <span data-ttu-id="e1126-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e1126-105">Partner Center</span></span>

<span data-ttu-id="e1126-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="e1126-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e1126-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e1126-107">Global admin</span></span>

<span data-ttu-id="e1126-108">Ajoutez simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e1126-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="e1126-109">Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e1126-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="e1126-110">Conditions requises pour les fichiers de données</span><span class="sxs-lookup"><span data-stu-id="e1126-110">Data file requirements</span></span>

<span data-ttu-id="e1126-111">Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="e1126-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="e1126-112">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="e1126-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="e1126-113">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="e1126-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="e1126-114">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="e1126-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="e1126-115">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="e1126-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="e1126-116">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="e1126-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="e1126-117">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e1126-117">Enter only the data described below.</span></span> <span data-ttu-id="e1126-118">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="e1126-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="e1126-119">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="e1126-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="e1126-120">**Nom de la colonne**</span><span class="sxs-lookup"><span data-stu-id="e1126-120">**Column name**</span></span> | <span data-ttu-id="e1126-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1126-121">**Description**</span></span>  | <span data-ttu-id="e1126-122">**Limite**</span><span class="sxs-lookup"><span data-stu-id="e1126-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="e1126-123">Prénom</span><span class="sxs-lookup"><span data-stu-id="e1126-123">First name</span></span>  | <span data-ttu-id="e1126-124">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="e1126-124">User's first name (optional field)</span></span>  | <span data-ttu-id="e1126-125">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="e1126-125">50-character limit</span></span>  |
| <span data-ttu-id="e1126-126">Nom</span><span class="sxs-lookup"><span data-stu-id="e1126-126">Last name</span></span>  | <span data-ttu-id="e1126-127">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="e1126-127">User's last name (optional field)</span></span>  | <span data-ttu-id="e1126-128">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="e1126-128">50-character limit</span></span>  |
| <span data-ttu-id="e1126-129">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="e1126-129">Display name</span></span>    | <span data-ttu-id="e1126-130">Nom affiché dans l’espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="e1126-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="e1126-131">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="e1126-131">50-character limit</span></span>                         |
| <span data-ttu-id="e1126-132">Courrier</span><span class="sxs-lookup"><span data-stu-id="e1126-132">Email</span></span>   | <span data-ttu-id="e1126-133">Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="e1126-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="e1126-134">Chaque utilisateur doit avoir une adresse e-mail unique</span><span class="sxs-lookup"><span data-stu-id="e1126-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="e1126-135">Mise à jour de l'état</span><span class="sxs-lookup"><span data-stu-id="e1126-135">Status update</span></span>   | <span data-ttu-id="e1126-136">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé</span><span class="sxs-lookup"><span data-stu-id="e1126-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="e1126-137">\*\*Conserver vide\*\*</span><span class="sxs-lookup"><span data-stu-id="e1126-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="e1126-138">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e1126-138">Next steps</span></span>

- [<span data-ttu-id="e1126-139">Ajout de plusieurs utilisateurs à un client</span><span class="sxs-lookup"><span data-stu-id="e1126-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)