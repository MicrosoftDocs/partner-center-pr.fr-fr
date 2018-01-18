---
title: "Créer plusieurs utilisateurs pour un compte client | Espace partenaires"
description: "Vous pouvez ajouter plusieurs utilisateurs en même temps au compte d’un client, en chargeant un fichier de donnéesCSV dans l’Espace partenaires."
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: "chargement groupé, ajouter plusieurs utilisateurs à un compte client, ajouter des utilisateurs du client, chargement groupé des utilisateurs du client, compte client, utilisateurs du client, utilisateurs"
ms.openlocfilehash: b360ced878973cde19b1a6aa8470ac4218ea6773
ms.sourcegitcommit: e01a63d8b778668c560bc821275ddfcb0a6d4881
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2017
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="6afea-104">Ajouter plusieurs utilisateurs à un compte client</span><span class="sxs-lookup"><span data-stu-id="6afea-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="6afea-105">S'applique à</span><span class="sxs-lookup"><span data-stu-id="6afea-105">Applies to</span></span>**

-  <span data-ttu-id="6afea-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6afea-106">Partner Center</span></span>

<span data-ttu-id="6afea-107">Vous pouvez ajouter plusieurs utilisateurs en même temps au compte d’un client, en chargeant un fichier de donnéesCSV dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6afea-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to Partner Center.</span></span> <span data-ttu-id="6afea-108">Vous pouvez télécharger un exemple de fichier de données à partir de l’Espace partenaires, puis l’adapter à votre utilisation, ou créer un fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="6afea-108">You can download a sample data file from Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="6afea-109">Conditions requises pour les fichiers de données</span><span class="sxs-lookup"><span data-stu-id="6afea-109">Data file requirements</span></span>


<span data-ttu-id="6afea-110">Pour ajouter plusieurs utilisateurs au compte d’un client par chargement groupé, vous devez respecter les conditions suivantes&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="6afea-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="6afea-111">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="6afea-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="6afea-112">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="6afea-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="6afea-113">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="6afea-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="6afea-114">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="6afea-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="6afea-115">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="6afea-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="6afea-116">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="6afea-116">Enter only the data described below.</span></span> <span data-ttu-id="6afea-117">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="6afea-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="6afea-118">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="6afea-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="6afea-119">Nom de la colonne</span><span class="sxs-lookup"><span data-stu-id="6afea-119">Column name</span></span>** | **<span data-ttu-id="6afea-120">Description</span><span class="sxs-lookup"><span data-stu-id="6afea-120">Description</span></span>**                                                              | **<span data-ttu-id="6afea-121">Limitation</span><span class="sxs-lookup"><span data-stu-id="6afea-121">Limitation</span></span>**                             |
| <span data-ttu-id="6afea-122">Prénom</span><span class="sxs-lookup"><span data-stu-id="6afea-122">First name</span></span>      | <span data-ttu-id="6afea-123">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="6afea-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="6afea-124">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="6afea-124">50-character limit</span></span>                         |
| <span data-ttu-id="6afea-125">Nom</span><span class="sxs-lookup"><span data-stu-id="6afea-125">Last name</span></span>       | <span data-ttu-id="6afea-126">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="6afea-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="6afea-127">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="6afea-127">50-character limit</span></span>                         |
| <span data-ttu-id="6afea-128">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="6afea-128">Display name</span></span>    | <span data-ttu-id="6afea-129">Nom affiché dans l’Espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="6afea-129">Name displayed in Partner Center (required field)</span></span>                            | <span data-ttu-id="6afea-130">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="6afea-130">50-character limit</span></span>                         |
| <span data-ttu-id="6afea-131">Email</span><span class="sxs-lookup"><span data-stu-id="6afea-131">Email</span></span>           | <span data-ttu-id="6afea-132">Adresse de messagerie professionnelle de l’utilisateur chez le client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="6afea-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="6afea-133">Chaque utilisateur doit avoir une adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="6afea-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="6afea-134">Mise à jour de l’état</span><span class="sxs-lookup"><span data-stu-id="6afea-134">Status update</span></span>   | <span data-ttu-id="6afea-135">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé.</span><span class="sxs-lookup"><span data-stu-id="6afea-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="6afea-136">\*\*Laisser vide\* \ *</span><span class="sxs-lookup"><span data-stu-id="6afea-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="6afea-137">Pour créer plusieurs comptes d’utilisateur&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="6afea-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="6afea-138">Créez un fichier de données&nbsp;CSV avec les données décrites ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="6afea-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="6afea-139">Enregistrez le fichier pour pouvoir le retrouver ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="6afea-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="6afea-140">Dans le menu **Tableau de bord**, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="6afea-140">From the **Dashboard** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="6afea-141">Sélectionnez **Charger des utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="6afea-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="6afea-142">Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.</span><span class="sxs-lookup"><span data-stu-id="6afea-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="6afea-143">Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="6afea-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="6afea-144">Sélectionnez **Valider**.</span><span class="sxs-lookup"><span data-stu-id="6afea-144">Select **Validate**.</span></span>

    <span data-ttu-id="6afea-145">**Remarque** La plupart des erreurs de création de compte sont provoquées par des problèmes de fichier de données, comme des informations manquantes, des adresses de messagerie incorrectes ou dupliquées, un trop grand nombre d’enregistrements dans le fichier.</span><span class="sxs-lookup"><span data-stu-id="6afea-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

     

7.  <span data-ttu-id="6afea-146">Lorsque l’Espace partenaires a validé le fichier, sélectionnez l’**emplacement** géographique des nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6afea-146">After Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="6afea-147">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="6afea-147">Select **Save**.</span></span>
9.  <span data-ttu-id="6afea-148">Téléchargez le mot de passe temporaire des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6afea-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="6afea-149">**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après.</span><span class="sxs-lookup"><span data-stu-id="6afea-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="6afea-150">Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.</span><span class="sxs-lookup"><span data-stu-id="6afea-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

<span data-ttu-id="6afea-151">L’Espace partenaires attribue automatiquement les autorisations **Peut utiliser les licences et services** aux nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6afea-151">Partner Center automatically assigns permissions of **Can use licenses and services** to the new users.</span></span>

 

 



