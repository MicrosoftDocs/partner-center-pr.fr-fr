---
title: Transférer des abonnements Azure | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Un client peut changer de partenaire dans le programme Fournisseur de solutions&nbsp;Cloud pour utiliser les services Microsoft&nbsp;Azure. Toutefois, ce processus manuel nécessite des actions de la part du partenaire et du client.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.author: evansma
keywords: abonnement Azure, changer de partenaire, trouver un nouveau partenaire, autre partenaire
ms.localizationpriority: medium
ms.openlocfilehash: f9df7ac6c1e30f9e0d9d62c5e0c18aae529c472a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584352"
---
# <a name="transfer-azure-subscriptions"></a>Transférer des abonnements Azure 

**S’applique à**

-  Espace partenaires

Un client peut décider de faire appel à un partenaire fournisseur de solutions Cloud ou à un autre partenaire pour utiliser les services Microsoft Azure. Toutefois, ce processus manuel nécessite des actions de la part du partenaire et du client.

>[!Note]  
>Pour l’instant uniquement Direct ou Indirect de fournisseurs sont en mesure de transférer les abonnements.
>Il n’est pas encore possible de modifier des partenaires pour les abonnements de fournisseur de solutions Cloud pour les abonnements Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.



**Partenaires de commutateur pour les abonnements Azure**

1. Pour transférer un abonnement Azure vers un nouveau partenaire, le client doit lancer le processus et contacter son partenaire de référence actuel par écrit. 
>[!Note]
>Il incombe au partenaire actuel de créer le ticket de service qui lance le processus de transfert. Microsoft ne peut pas intervenir pour le compte du client ou du nouveau partenaire. Le client doit prévoir de collaborer étroitement avec le partenaire actuel pour que la transition se passe sans heurt.

2. Le partenaire de l'abonnement doit effectuer les tâches suivantes :

Créez un ticket de service Azure dans l’Espace partenaires pour demander un transfert d’abonnement&nbsp;:
-   Dans le menu espace partenaires, sélectionnez **clients**, sélectionnez votre client à partir de la liste, puis **gestion des services**. Dans la section **Tickets de support**, cliquez sur le menu déroulant **Nouveau ticket** et choisissez **Microsoft Azure**.

-   Dans le portail Azure, sélectionnez **Nouvelle demande de support**.

À l’étape&nbsp;1, choisissez le type de problème **Gestion des abonnements**, indiquez l’ID d’abonnement que vous voulez transférer, puis choisissez **Fournisseur de solutions&nbsp;Cloud** comme formule d’assistance.

À l’étape 2, sélectionnez **C - Impact minime** et choisissez le type de problème **Autres questions générales**.

Téléchargez le [formulaire de transfert d’abonnement Fournisseur de solutions&nbsp;Cloud](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. Le partenaire pour l’abonnement : Renseignez le [formulaire de transfert d’abonnement CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), signez-le et envoyez-le au client. Pour remplir le formulaire, vous aurez besoin des informations suivantes&nbsp;:

- Les coordonnées du partenaire actuel et son ID Microsoft. Dans le menu espace partenaires, sélectionnez **paramètres du compte** &gt; **profil organisation**et utiliser le **ID Microsoft**, **nom de l’organisation** , et **adresse** y figurent.

- L’ID&nbsp;Microsoft du client. Dans le menu de l’Espace partenaires, sélectionnez **Clients**, puis développez la page de description du client pour voir son **ID&nbsp;Microsoft**.

- L’ID d’abonnement à transférer. Dans la page de description développée du client, sélectionnez **Afficher les abonnements**, puis développez l’abonnement choisi pour voir son **ID d’abonnement**.

>[!Note]
>Transfert d’un abonnement entraîne deux abonnement ID qui s’affiche sur le **modifier l’abonnement** page de l’abonnement transférée : **1**-l’ID d’abonnement Partner Center est utilisé à des fins de facturation. 
**2**- L'ID d’abonnement Azure original est conservé et apparaîtra dans l'Espace partenaires, ainsi que dans le portail de gestion Azure. Cet ID apparaîtra dans votre fichier de rapprochement.  **Quand vous vous connectez des tickets de support, vous devez utiliser ces deux ID.**

4. Le client et le nouveau partenaire de l'abonnement :

Vérifiez le formulaire, renseignez les informations sur le nouveau partenaire, puis signez-le. Vérifiez que le nouveau client dispose d’un accord de contrat. Renvoyez le formulaire au partenaire de référence actuel.

*Important* : Si le nouveau partenaire CSP n’a pas d’une relation de revendeur avec le client, elles doivent établir une avant de l’abonnement en cours de transfert. [Pour plus d’informations sur la marche à suivre, cliquez ici](request-a-relationship-with-a-customer.md).

>[!Note]
>Le nouveau partenaire CSP et au client doivent être dans le même pays. 

5. Partenaire actuel :

Vérifiez que le formulaire indique les coordonnées des deux&nbsp;administrateurs du partenaire. Le support Microsoft les contactera tous les deux pour confirmer le transfert. Assurez-vous que les trois signatures sont présentes et joignez le formulaire rempli à votre demande de service existante à l’aide de l’option **Chargement de fichier**. Un ingénieur du support Microsoft vous contactera sous 8&nbsp;heures ouvrées pour valider la réception et l’achèvement.

6. Nouveau partenaire :

Modifiez les paramètres d’abonnement Azure en supprimant l’ancien partenaire du compte. Pour afficher les attributions de rôle approvisionnées, exécutez deux applets de commande Powershell.

-   Ajoutez le nouveau partenaire comme revendeur sur le compte :

**PS C :\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

Pour trouver le customerDomainName : dans le menu de l’Espace partenaires, sélectionnez **Clients**. Dans la liste des clients, sélectionnez le client. Dans le menu client, sélectionnez **Compte** et utilisez le **Nom de domaine**.

-   Affichez les rôles du compte, y compris les anciens partenaires Fournisseur de solutions Cloud :

**PS C :\\&gt; Get-AzureRMRoleAssignment**

7. Supprimer des autorisations d'accès obsolètes

-  Dans le menu de l’Espace partenaires, sélectionnez **Clients**. 
-  Développez la page de description et sélectionnez **Afficher les abonnements**. 
-  Dans le menu client, sélectionnez **Gestion des services**. 
-  Sous **Microsoft&nbsp;Azure**, cliquez sur le lien pour accéder au **portail de gestion Microsoft&nbsp;Azure**.

 

 



