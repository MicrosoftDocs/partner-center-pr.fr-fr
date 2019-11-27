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
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="a9869-104">Ajouter plusieurs utilisateurs à un compte client</span><span class="sxs-lookup"><span data-stu-id="a9869-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="a9869-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="a9869-105">**Applies to**</span></span>

-  <span data-ttu-id="a9869-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a9869-106">Partner Center</span></span>

<span data-ttu-id="a9869-107">Vous pouvez ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a9869-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="a9869-108">Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a9869-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="a9869-109">Exigences relatives aux fichiers de données</span><span class="sxs-lookup"><span data-stu-id="a9869-109">Data file requirements</span></span>


<span data-ttu-id="a9869-110">Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="a9869-110">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

-   <span data-ttu-id="a9869-111">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="a9869-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="a9869-112">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="a9869-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="a9869-113">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="a9869-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="a9869-114">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="a9869-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="a9869-115">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="a9869-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="a9869-116">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a9869-116">Enter only the data described below.</span></span> <span data-ttu-id="a9869-117">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="a9869-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="a9869-118">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="a9869-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="a9869-119">**Nom de la colonne**</span><span class="sxs-lookup"><span data-stu-id="a9869-119">**Column name**</span></span> | <span data-ttu-id="a9869-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="a9869-120">**Description**</span></span>                                                              | <span data-ttu-id="a9869-121">**Contrainte**</span><span class="sxs-lookup"><span data-stu-id="a9869-121">**Limitation**</span></span>                             |
| <span data-ttu-id="a9869-122">Prénom</span><span class="sxs-lookup"><span data-stu-id="a9869-122">First name</span></span>      | <span data-ttu-id="a9869-123">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="a9869-123">User's first name (optional field)</span></span>                                           | <span data-ttu-id="a9869-124">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="a9869-124">50-character limit</span></span>                         |
| <span data-ttu-id="a9869-125">Nom</span><span class="sxs-lookup"><span data-stu-id="a9869-125">Last name</span></span>       | <span data-ttu-id="a9869-126">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="a9869-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="a9869-127">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="a9869-127">50-character limit</span></span>                         |
| <span data-ttu-id="a9869-128">Display name</span><span class="sxs-lookup"><span data-stu-id="a9869-128">Display name</span></span>    | <span data-ttu-id="a9869-129">Nom affiché dans l’espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="a9869-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="a9869-130">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="a9869-130">50-character limit</span></span>                         |
| <span data-ttu-id="a9869-131">E-mail</span><span class="sxs-lookup"><span data-stu-id="a9869-131">Email</span></span>           | <span data-ttu-id="a9869-132">Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="a9869-132">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="a9869-133">Chaque utilisateur doit avoir une adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="a9869-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="a9869-134">Mise à jour de l’état</span><span class="sxs-lookup"><span data-stu-id="a9869-134">Status update</span></span>   | <span data-ttu-id="a9869-135">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé</span><span class="sxs-lookup"><span data-stu-id="a9869-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="a9869-136">\*\*laissez un\*vide \*</span><span class="sxs-lookup"><span data-stu-id="a9869-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="a9869-137">Pour créer plusieurs comptes d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a9869-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="a9869-138">Créez un fichier de données CSV avec les données décrites ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="a9869-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="a9869-139">Enregistrez le fichier pour pouvoir le retrouver ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="a9869-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="a9869-140">Dans le menu **espace partenaires** , sélectionnez **clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9869-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="a9869-141">Sélectionnez **Charger des utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="a9869-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="a9869-142">Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.</span><span class="sxs-lookup"><span data-stu-id="a9869-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="a9869-143">Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="a9869-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="a9869-144">Sélectionnez **Valider**.</span><span class="sxs-lookup"><span data-stu-id="a9869-144">Select **Validate**.</span></span>

    <span data-ttu-id="a9869-145">**Notez**  la plupart des erreurs de création de compte sont provoquées par des problèmes de fichiers de données, notamment des informations manquantes, des adresses de messagerie incorrectes ou en double ou des enregistrements trop nombreux dans le fichier.</span><span class="sxs-lookup"><span data-stu-id="a9869-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="a9869-146">Une fois que l’espace partenaires a validé le fichier, sélectionnez l' **emplacement** géographique pour les nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="a9869-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="a9869-147">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="a9869-147">Select **Save**.</span></span>
9.  <span data-ttu-id="a9869-148">Téléchargez le mot de passe temporaire des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="a9869-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="a9869-149">**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après.</span><span class="sxs-lookup"><span data-stu-id="a9869-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="a9869-150">Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.</span><span class="sxs-lookup"><span data-stu-id="a9869-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="a9869-151">Les autorisations **Peut utiliser les licences et services** sont automatiquement attribuées aux nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="a9869-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



