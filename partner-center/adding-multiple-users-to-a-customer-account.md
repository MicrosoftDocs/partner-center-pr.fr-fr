---
title: Créer plusieurs utilisateurs pour un compte client | Espace partenaires
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: jasonwhowell
ms.author: jasonh
keywords: chargement groupé, ajouter plusieurs utilisateurs à un compte client, ajouter des utilisateurs du client, chargement groupé des utilisateurs du client, compte client, utilisateurs du client, utilisateurs
ms.localizationpriority: medium
ms.openlocfilehash: 499aff67d18b0d8f9fbaf098fecbab2d888d9ac7
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390368"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="cdb8c-104">Ajouter plusieurs utilisateurs à un compte client</span><span class="sxs-lookup"><span data-stu-id="cdb8c-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="cdb8c-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="cdb8c-105">**Applies to**</span></span>

- <span data-ttu-id="cdb8c-106">Centre pour partenaires</span><span class="sxs-lookup"><span data-stu-id="cdb8c-106">Partner Center</span></span>

<span data-ttu-id="cdb8c-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="cdb8c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="cdb8c-108">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="cdb8c-108">Global admin</span></span>

<span data-ttu-id="cdb8c-109">Vous pouvez ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="cdb8c-110">Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="cdb8c-111">Exigences relatives aux fichiers de données</span><span class="sxs-lookup"><span data-stu-id="cdb8c-111">Data file requirements</span></span>

<span data-ttu-id="cdb8c-112">Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="cdb8c-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="cdb8c-113">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="cdb8c-114">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="cdb8c-115">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="cdb8c-116">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="cdb8c-117">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="cdb8c-118">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-118">Enter only the data described below.</span></span> <span data-ttu-id="cdb8c-119">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="cdb8c-120">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="cdb8c-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="cdb8c-121">**Nom de la colonne**</span><span class="sxs-lookup"><span data-stu-id="cdb8c-121">**Column name**</span></span> | <span data-ttu-id="cdb8c-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="cdb8c-122">**Description**</span></span>                                                              | <span data-ttu-id="cdb8c-123">**Contrainte**</span><span class="sxs-lookup"><span data-stu-id="cdb8c-123">**Limitation**</span></span>                             |
| <span data-ttu-id="cdb8c-124">Prénom</span><span class="sxs-lookup"><span data-stu-id="cdb8c-124">First name</span></span>      | <span data-ttu-id="cdb8c-125">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="cdb8c-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="cdb8c-126">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="cdb8c-126">50-character limit</span></span>                         |
| <span data-ttu-id="cdb8c-127">Nom</span><span class="sxs-lookup"><span data-stu-id="cdb8c-127">Last name</span></span>       | <span data-ttu-id="cdb8c-128">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="cdb8c-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="cdb8c-129">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="cdb8c-129">50-character limit</span></span>                         |
| <span data-ttu-id="cdb8c-130">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="cdb8c-130">Display name</span></span>    | <span data-ttu-id="cdb8c-131">Nom affiché dans l’espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="cdb8c-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="cdb8c-132">50&nbsp;caractères maximum</span><span class="sxs-lookup"><span data-stu-id="cdb8c-132">50-character limit</span></span>                         |
| <span data-ttu-id="cdb8c-133">E-mail</span><span class="sxs-lookup"><span data-stu-id="cdb8c-133">Email</span></span>           | <span data-ttu-id="cdb8c-134">Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="cdb8c-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="cdb8c-135">Chaque utilisateur doit avoir une adresse de messagerie unique.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="cdb8c-136">Mise à jour de l’état</span><span class="sxs-lookup"><span data-stu-id="cdb8c-136">Status update</span></span>   | <span data-ttu-id="cdb8c-137">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé</span><span class="sxs-lookup"><span data-stu-id="cdb8c-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="cdb8c-138">\*\*laissez un\*vide \*</span><span class="sxs-lookup"><span data-stu-id="cdb8c-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="cdb8c-139">Pour créer plusieurs comptes d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="cdb8c-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="cdb8c-140">Créez un fichier de données CSV avec les données décrites ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="cdb8c-141">Enregistrez le fichier pour pouvoir le retrouver ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="cdb8c-142">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="cdb8c-143">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="cdb8c-144">Sélectionnez l’onglet **utilisateurs et licences** du client, puis cliquez sur **Télécharger les utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="cdb8c-145">Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="cdb8c-146">Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="cdb8c-147">Sélectionnez **Valider**.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-147">Select **Validate**.</span></span>

    <span data-ttu-id="cdb8c-148">**Notez**  la plupart des erreurs de création de compte sont provoquées par des problèmes de fichiers de données, notamment des informations manquantes, des adresses de messagerie incorrectes ou en double ou des enregistrements trop nombreux dans le fichier.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="cdb8c-149">Une fois que l’espace partenaires a validé le fichier, sélectionnez l' **emplacement** géographique pour les nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="cdb8c-150">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-150">Select **Save**.</span></span>
10. <span data-ttu-id="cdb8c-151">Téléchargez le mot de passe temporaire des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="cdb8c-152">**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="cdb8c-153">Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="cdb8c-154">Les autorisations **Peut utiliser les licences et services** sont automatiquement attribuées aux nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="cdb8c-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



