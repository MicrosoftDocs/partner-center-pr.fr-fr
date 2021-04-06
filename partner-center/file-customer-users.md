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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441419"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="8886f-103">Ajouter plusieurs utilisateurs à un compte client en créant un fichier. csv</span><span class="sxs-lookup"><span data-stu-id="8886f-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="8886f-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="8886f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8886f-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="8886f-105">Global admin</span></span>

<span data-ttu-id="8886f-106">Ajoutez simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8886f-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="8886f-107">Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8886f-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="8886f-108">Conditions requises pour les fichiers de données</span><span class="sxs-lookup"><span data-stu-id="8886f-108">Data file requirements</span></span>

<span data-ttu-id="8886f-109">Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="8886f-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="8886f-110">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="8886f-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="8886f-111">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="8886f-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="8886f-112">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="8886f-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="8886f-113">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="8886f-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="8886f-114">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="8886f-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="8886f-115">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8886f-115">Enter only the data described below.</span></span> <span data-ttu-id="8886f-116">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="8886f-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="8886f-117">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="8886f-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="8886f-118">**Nom de la colonne**</span><span class="sxs-lookup"><span data-stu-id="8886f-118">**Column name**</span></span> | <span data-ttu-id="8886f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="8886f-119">**Description**</span></span>  | <span data-ttu-id="8886f-120">**Limite**</span><span class="sxs-lookup"><span data-stu-id="8886f-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="8886f-121">Prénom</span><span class="sxs-lookup"><span data-stu-id="8886f-121">First name</span></span>  | <span data-ttu-id="8886f-122">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="8886f-122">User's first name (optional field)</span></span>  | <span data-ttu-id="8886f-123">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="8886f-123">50-character limit</span></span>  |
| <span data-ttu-id="8886f-124">Nom</span><span class="sxs-lookup"><span data-stu-id="8886f-124">Last name</span></span>  | <span data-ttu-id="8886f-125">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="8886f-125">User's last name (optional field)</span></span>  | <span data-ttu-id="8886f-126">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="8886f-126">50-character limit</span></span>  |
| <span data-ttu-id="8886f-127">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="8886f-127">Display name</span></span>    | <span data-ttu-id="8886f-128">Nom affiché dans l’espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="8886f-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="8886f-129">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="8886f-129">50-character limit</span></span>                         |
| <span data-ttu-id="8886f-130">Email</span><span class="sxs-lookup"><span data-stu-id="8886f-130">Email</span></span>   | <span data-ttu-id="8886f-131">Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="8886f-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="8886f-132">Chaque utilisateur doit avoir une adresse e-mail unique</span><span class="sxs-lookup"><span data-stu-id="8886f-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="8886f-133">Mise à jour de l'état</span><span class="sxs-lookup"><span data-stu-id="8886f-133">Status update</span></span>   | <span data-ttu-id="8886f-134">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé avec succès</span><span class="sxs-lookup"><span data-stu-id="8886f-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="8886f-135">\*\*Conserver vide\*\*</span><span class="sxs-lookup"><span data-stu-id="8886f-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="8886f-136">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8886f-136">Next steps</span></span>

- [<span data-ttu-id="8886f-137">Guide pratique pour ajouter plusieurs utilisateurs pour un client</span><span class="sxs-lookup"><span data-stu-id="8886f-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)