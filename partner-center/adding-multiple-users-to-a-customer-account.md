---
title: Ajouter plusieurs utilisateurs pour un compte client
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter simultanément plusieurs utilisateurs au compte d’un client. Téléchargez un fichier de données dans l’espace partenaires à l’aide du format de fichier de valeurs séparées par des virgules (. csv).
author: LauraBrenner
ms.author: labrenne
keywords: le chargement en bloc, l’ajout de plusieurs utilisateurs au compte d’un client, l’ajout d’utilisateurs du client, le téléchargement en bloc des utilisateurs du client, le compte client, les utilisateurs clients, les utilisateurs
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44e8da91a622fe640e9e41f8d8d464a61652ef30
ms.sourcegitcommit: f71963d6a7ced48ea73580fa57f559ae69f31940
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/19/2020
ms.locfileid: "85104120"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="d8bc6-105">Ajouter plusieurs utilisateurs à un compte client-charger un fichier de données dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d8bc6-105">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="d8bc6-106">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="d8bc6-106">**Applies to**</span></span>

- <span data-ttu-id="d8bc6-107">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d8bc6-107">Partner Center</span></span>

<span data-ttu-id="d8bc6-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="d8bc6-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d8bc6-109">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="d8bc6-109">Global admin</span></span>

<span data-ttu-id="d8bc6-110">Vous pouvez ajouter simultanément plusieurs utilisateurs au compte d’un client, en chargeant un fichier de données au format de fichier de valeurs séparées par des virgules (. csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-110">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="d8bc6-111">Vous pouvez télécharger un exemple de fichier de données à partir de l’espace partenaires, puis le modifier pour votre utilisation, ou vous pouvez créer un nouveau fichier de données à l’aide du modèle de données défini ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-111">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="d8bc6-112">Conditions requises pour les fichiers de données</span><span class="sxs-lookup"><span data-stu-id="d8bc6-112">Data file requirements</span></span>

<span data-ttu-id="d8bc6-113">Pour ajouter plusieurs utilisateurs au compte d’un client à l’aide du processus de téléchargement en bloc, vous devez respecter les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="d8bc6-113">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="d8bc6-114">Vous devez posséder des autorisations d’administrateur global sur le compte client.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-114">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="d8bc6-115">Chaque utilisateur doit avoir une adresse de messagerie unique, ajoutée à un ou plusieurs domaines de messagerie du client.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-115">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="d8bc6-116">Vous pouvez charger jusqu’à 100&nbsp;enregistrements à la fois.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-116">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="d8bc6-117">Si vous avez besoin d’ajouter plus de 100&nbsp;utilisateurs, créez et chargez des fichiers de données supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-117">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="d8bc6-118">Tous les utilisateurs doivent se trouver dans le même **emplacement** géographique.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-118">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="d8bc6-119">N’entrez que les données décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-119">Enter only the data described below.</span></span> <span data-ttu-id="d8bc6-120">Les autres données bloqueront le chargement.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-120">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="d8bc6-121">Entrez les données suivantes dans le fichier de données&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="d8bc6-121">Enter the following data in the data file:</span></span>

| <span data-ttu-id="d8bc6-122">**Nom de la colonne**</span><span class="sxs-lookup"><span data-stu-id="d8bc6-122">**Column name**</span></span> | <span data-ttu-id="d8bc6-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8bc6-123">**Description**</span></span>  | <span data-ttu-id="d8bc6-124">**Limite**</span><span class="sxs-lookup"><span data-stu-id="d8bc6-124">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="d8bc6-125">Prénom</span><span class="sxs-lookup"><span data-stu-id="d8bc6-125">First name</span></span>  | <span data-ttu-id="d8bc6-126">Prénom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="d8bc6-126">User's first name (optional field)</span></span>  | <span data-ttu-id="d8bc6-127">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="d8bc6-127">50-character limit</span></span>  |
| <span data-ttu-id="d8bc6-128">Nom</span><span class="sxs-lookup"><span data-stu-id="d8bc6-128">Last name</span></span>  | <span data-ttu-id="d8bc6-129">Nom de l’utilisateur (champ facultatif)</span><span class="sxs-lookup"><span data-stu-id="d8bc6-129">User's last name (optional field)</span></span>  | <span data-ttu-id="d8bc6-130">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="d8bc6-130">50-character limit</span></span>  |
| <span data-ttu-id="d8bc6-131">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="d8bc6-131">Display name</span></span>    | <span data-ttu-id="d8bc6-132">Nom affiché dans l’espace partenaires (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="d8bc6-132">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="d8bc6-133">limité à 50 caractères</span><span class="sxs-lookup"><span data-stu-id="d8bc6-133">50-character limit</span></span>                         |
| <span data-ttu-id="d8bc6-134">E-mail</span><span class="sxs-lookup"><span data-stu-id="d8bc6-134">Email</span></span>   | <span data-ttu-id="d8bc6-135">Adresse de messagerie professionnelle de l’utilisateur dans la société du client (champ obligatoire)</span><span class="sxs-lookup"><span data-stu-id="d8bc6-135">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="d8bc6-136">Chaque utilisateur doit avoir une adresse e-mail unique</span><span class="sxs-lookup"><span data-stu-id="d8bc6-136">Each user must have a unique email address</span></span> |
| <span data-ttu-id="d8bc6-137">Mise à jour de l'état</span><span class="sxs-lookup"><span data-stu-id="d8bc6-137">Status update</span></span>   | <span data-ttu-id="d8bc6-138">Permet d’indiquer si le nouvel enregistrement d’utilisateur a été créé</span><span class="sxs-lookup"><span data-stu-id="d8bc6-138">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="d8bc6-139">\*\*Conserver vide\*\*</span><span class="sxs-lookup"><span data-stu-id="d8bc6-139">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="d8bc6-140">Pour créer plusieurs comptes d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d8bc6-140">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="d8bc6-141">Créez un fichier de données CSV avec les données décrites ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-141">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="d8bc6-142">Enregistrez le fichier pour pouvoir le retrouver ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-142">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="d8bc6-143">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="d8bc6-144">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-144">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="d8bc6-145">Sélectionnez l’onglet **utilisateurs et licences** du client, puis cliquez sur **Télécharger les utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-145">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="d8bc6-146">Sous **Charger des informations d’utilisateur**, sélectionnez **Parcourir**.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-146">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="d8bc6-147">Dans le sélecteur de fichiers, sélectionnez votre fichier de données, puis **Ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-147">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="d8bc6-148">Sélectionnez **Valider**.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-148">Select **Validate**.</span></span>

    <span data-ttu-id="d8bc6-149">**Remarque**    La plupart des erreurs de création de compte sont provoquées par des problèmes de fichiers de données, notamment des informations manquantes, des adresses de messagerie incorrectes ou en double ou des enregistrements trop nombreux dans le fichier.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-149">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="d8bc6-150">Une fois que l’espace partenaires a validé le fichier, sélectionnez l' **emplacement** géographique pour les nouveaux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-150">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="d8bc6-151">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-151">Select **Save**.</span></span>
10. <span data-ttu-id="d8bc6-152">Chargez les informations sur le mot de passe temporaire pour les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-152">Download the temporary password information for the users.</span></span>

<span data-ttu-id="d8bc6-153">**IMPORTANT&nbsp;:** n’oubliez pas de télécharger le fichier avec les mots de passe temporaires maintenant, car cette opération ne sera plus possible après.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-153">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="d8bc6-154">Les nouveaux utilisateurs doivent se connecter à leur nouveau compte à l’aide du mot de passe temporaire correspondant.</span><span class="sxs-lookup"><span data-stu-id="d8bc6-154">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="d8bc6-155">Les autorisations qui sont attribuées automatiquement aux nouveaux utilisateurs **peuvent utiliser des licences et des services** .</span><span class="sxs-lookup"><span data-stu-id="d8bc6-155">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



