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
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="48d14-103">Ajouter plusieurs utilisateurs à un compte client en créant un fichier. csv</span><span class="sxs-lookup"><span data-stu-id="48d14-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="48d14-104">**Rôles appropriés** : administrateur général</span><span class="sxs-lookup"><span data-stu-id="48d14-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="48d14-105">Ajoutez simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="48d14-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="48d14-106">Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="48d14-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="48d14-107">Conditions requises pour les fichiers de données</span><span class="sxs-lookup"><span data-stu-id="48d14-107">Data file requirements</span></span>

<span data-ttu-id="48d14-108">Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="48d14-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="48d14-109">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="48d14-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="48d14-110">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="48d14-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="48d14-111">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="48d14-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="48d14-112">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="48d14-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="48d14-113">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="48d14-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="48d14-114">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="48d14-114">Enter only the data described below.</span></span> <span data-ttu-id="48d14-115">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="48d14-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="48d14-116">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="48d14-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="48d14-117">**Nom de la colonne**</span><span class="sxs-lookup"><span data-stu-id="48d14-117">**Column name**</span></span> | <span data-ttu-id="48d14-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="48d14-118">**Description**</span></span>  | <span data-ttu-id="48d14-119">**Limite**</span><span class="sxs-lookup"><span data-stu-id="48d14-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="48d14-120">Prénom</span><span class="sxs-lookup"><span data-stu-id="48d14-120">First name</span></span>  | <span data-ttu-id="48d14-121">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="48d14-121">User's first name (optional field)</span></span>  | <span data-ttu-id="48d14-122">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="48d14-122">50-character limit</span></span>  |
| <span data-ttu-id="48d14-123">Nom</span><span class="sxs-lookup"><span data-stu-id="48d14-123">Last name</span></span>  | <span data-ttu-id="48d14-124">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="48d14-124">User's last name (optional field)</span></span>  | <span data-ttu-id="48d14-125">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="48d14-125">50-character limit</span></span>  |
| <span data-ttu-id="48d14-126">Nom complet</span><span class="sxs-lookup"><span data-stu-id="48d14-126">Display name</span></span>    | <span data-ttu-id="48d14-127">Nom affiché dans l’espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="48d14-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="48d14-128">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="48d14-128">50-character limit</span></span>                         |
| <span data-ttu-id="48d14-129">Courrier</span><span class="sxs-lookup"><span data-stu-id="48d14-129">Email</span></span>   | <span data-ttu-id="48d14-130">Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="48d14-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="48d14-131">Chaque utilisateur doit avoir une adresse e-mail unique</span><span class="sxs-lookup"><span data-stu-id="48d14-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="48d14-132">Mise à jour de l'état</span><span class="sxs-lookup"><span data-stu-id="48d14-132">Status update</span></span>   | <span data-ttu-id="48d14-133">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé avec succès</span><span class="sxs-lookup"><span data-stu-id="48d14-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="48d14-134">\*\*Conserver vide\*\*</span><span class="sxs-lookup"><span data-stu-id="48d14-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="48d14-135">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="48d14-135">Next steps</span></span>

- [<span data-ttu-id="48d14-136">Guide pratique pour ajouter plusieurs utilisateurs pour un client</span><span class="sxs-lookup"><span data-stu-id="48d14-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)