---
title: Transférer des abonnements Azure | Espace partenaires
description: Un client peut changer de partenaire dans le programme Fournisseur de solutions&nbsp;Cloud pour utiliser les services Microsoft&nbsp;Azure. Toutefois, ce processus manuel nécessite des actions de la part du partenaire et du client.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
keywords: abonnement Azure, changer de partenaire, trouver un nouveau partenaire, autre partenaire
ms.openlocfilehash: a4b9c0a320808f1d8a4a630a035660813a3f9c74
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2018
ms.locfileid: "2088956"
---
# <a name="transfer-azure-subscriptions"></a>Transférer des abonnements Azure 

**S'applique à**

-  Espace partenaires

Un client peut décider de faire appel à un partenaire fournisseur de solutions Cloud ou à un autre partenaire pour utiliser les services Microsoft Azure. Toutefois, ce processus manuel nécessite des actions de la part du partenaire et du client.

**Remarque** il n'est pas possible de changer de fournisseur de solutions Cloud pour les abonnements Office365, EnterpriseMobility ou MicrosoftDynamicsCRM.



**Changer de partenaire pour les abonnements Azure**

1.  Pour transférer un abonnement Azure vers un nouveau partenaire, le client doit lancer le processus et contacter son partenaire de référence actuel par écrit. 

    >**Remarque**<br> Il incombe au partenaire actuel de créer le ticket de service qui lance le processus de transfert. Microsoft ne peut pas intervenir pour le compte du client ou du nouveau partenaire. Le client doit prévoir de collaborer étroitement avec le partenaire actuel pour que la transition se passe sans heurt.

2.  Le partenaire de l'abonnement doit effectuer les tâches suivantes:

    Créez un ticket de service Azure dans l'Espace partenaires pour demander un transfert d'abonnement&nbsp;:

    -   Dans le menu Tableau de bord, sélectionnez **Clients**, choisissez votre client dans la liste, puis cliquez sur **Gestion des services**. Dans la section **Tickets de support**, cliquez sur le menu déroulant **Nouveau ticket** et choisissez **Microsoft Azure**.

    -   Dans le portail Azure, sélectionnez **Nouvelle demande de support**.

        À l'étape&nbsp;1, choisissez le type de problème **Gestion des abonnements**, indiquez l'ID d'abonnement que vous voulez transférer, puis choisissez **Fournisseur de solutions&nbsp;Cloud** comme formule d'assistance.

        À l'étape 2, sélectionnez **C - Impact minime** et choisissez le type de problème **Autres questions générales**.

        Télécharger le [formulaire de transfert d'abonnement Fournisseur de solutionsCloud](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  Partenaire Fournisseur de solutionsCloud de l'abonnement: remplissez le [formulaire de transfert d'abonnement Fournisseur de solutionsCloud](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), signez-le, puis envoyez-le au client. Pour remplir le formulaire, vous aurez besoin des informations suivantes&nbsp;:

    -   Les coordonnées du partenaire actuel et son ID Microsoft. Dans le menu de l'Espace partenaires, sélectionnez **Paramètres du compte** &gt; **Profil d'entreprise**, et utilisez les informations **ID Microsoft**, **Nom de l'organisation** et **Adresse** indiquées ici.

    -   L'ID&nbsp;Microsoft du client. Dans le menu de l'Espace partenaires, sélectionnez **Clients**, puis développez la page de description du client pour voir son **ID&nbsp;Microsoft**.

    -   L'ID d'abonnement à transférer. Dans la page de description développée du client, sélectionnez **Afficher les abonnements**, puis développez l'abonnement choisi pour voir son **ID d'abonnement**.

    >**Remarque**<br> Le transfert d’un abonnement entraîne la création de deux ID d'abonnement, visibles sur la page **Modifier un abonnement** de l’abonnement transféré: **1**- L’ID d’abonnement associé à l'Espace partenaires est utilisé pour la facturation. 
    **2**- L'ID d’abonnement Azure original est conservé et apparaîtra dans l'Espace partenaires, ainsi que dans le portail de gestion Azure. Cet ID apparaîtra dans votre fichier de rapprochement.  **Vous devez utiliser les deux ID pour toute soumission de ticket de support.**

4.  Le client et le nouveau partenaire de l'abonnement:

    Vérifient le formulaire, renseignent les informations sur le nouveau partenaire, puis le signent. Vérifiez que le nouveau client dispose d'un accord de contrat. Renvoyez le formulaire au partenaire de référence actuel.

    *Important*&nbsp;: si le nouveau partenaire Fournisseur de solutions&nbsp;Cloud n'a pas de relation de revendeur avec le client, il doit en établir une avant le transfert de l'abonnement. [Pour plus d'informations sur la marche à suivre, cliquez ici](request-a-relationship-with-a-customer.md).

5.  Partenaire actuel:

    Vérifiez que le formulaire indique les coordonnées des deux administrateurs du partenaire. Le support Microsoft les contactera tous les deux pour confirmer le transfert. Assurez-vous que les trois signatures sont présentes et joignez le formulaire rempli à votre demande de service existante à l'aide de l'option **Chargement de fichier**. Un ingénieur du support Microsoft vous contactera sous 8heures ouvrées pour valider la réception et l'achèvement.

6.  Nouveau partenaire:

    Modifiez les paramètres d'abonnement Azure en supprimant l'ancien partenaire du compte. Pour afficher les attributions de rôle approvisionnées, exécutez deux applets de commande Powershell.

    -   Ajoutez le nouveau partenaire comme revendeur sur le compte&nbsp;:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        Pour trouver le customerDomainName&nbsp;: dans le menu de l'Espace partenaires, sélectionnez **Clients**. Dans la liste des clients, sélectionnez le client. Dans le menu client, sélectionnez **Compte** et utilisez le **Nom de domaine**.

    -   Affichez les rôles du compte, y compris les anciens partenaires Fournisseur de solutions&nbsp;Cloud&nbsp;:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Supprimer des autorisations d'accès obsolètes

    -  Dans le menu de l'Espace partenaires, sélectionnez **Clients**. 
    -  Développez la page de description et sélectionnez **Afficher les abonnements**. 
    -  Dans le menu client, sélectionnez **Gestion des services**. 
    -  Sous **Microsoft&nbsp;Azure**, cliquez sur le lien pour accéder au **portail de gestion Microsoft&nbsp;Azure**.

 

 



