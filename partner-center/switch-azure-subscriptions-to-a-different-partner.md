---
title: "Transférer des abonnements Azure vers un autre partenaire | Espace partenaires"
description: "Un client peut changer de partenaire dans le programme Fournisseur de solutionsCloud pour utiliser les services MicrosoftAzure. Toutefois, ce processus manuel nécessite des actions de la part du partenaire et du client."
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 29ced9a3a7256f86f0f8708a4c72ac75b9269ffc

---

# Transférer un abonnement Azure vers un autre partenaire


Un client peut changer de partenaire dans le programme Fournisseur de solutionsCloud pour utiliser les services MicrosoftAzure. Toutefois, ce processus manuel nécessite des actions de la part du partenaire et du client.

**Remarque** Pour l’instant, aucune procédure automatique ne permet aux clients Azure de basculer des programmes de licence EA, Open ou autre vers le programme Fournisseur de solutionsCloud. Ce processus manuel nécessite des actions de la part du partenaire et du client. De plus, il n’est pas possible de changer de fournisseur de solutionsCloud pour les abonnements Office365, EnterpriseMobility ou MicrosoftDynamicsCRM.

 

**Changer de partenaire pour les abonnements Azure**

1.  Pour transférer un abonnement Azure vers un nouveau partenaire, le client doit lancer le processus et contacter son partenaire Fournisseur de solutionsCloud de référence par écrit.

2.  Le fournisseur de solutionsCloud de l’abonnement doit effectuer les tâches suivantes:

    Créez un ticket de service Azure dans l’Espace partenaires pour demander un transfert d’abonnement:

    -   Dans le menu Tableau de bord de l’Espace partenaires, sélectionnez **Clients**, choisissez votre client dans la liste, puis cliquez sur **Gestion des services**. Dans la section **Tickets de support**, cliquez sur le menu déroulant **Nouveau ticket** et choisissez **Microsoft Azure**.

    -   Dans le portail Azure, sélectionnez **Nouvelle demande de support**.

        À l’étape1, choisissez le type de problème **Gestion des abonnements**, indiquez l’ID d’abonnement que vous voulez transférer, puis choisissez **Fournisseur de solutionsCloud** comme formule d’assistance.

        À l’étape 2, sélectionnez **C - Impact minime** et choisissez le type de problème **Autres questions générales**.

        Téléchargez le [formulaire de transfert d’abonnement Fournisseur de solutionsCloud](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  Partenaire Fournisseur de solutionsCloud actuel de l’abonnement: remplissez le [formulaire de transfert d’abonnement Fournisseur de solutionsCloud](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), signez-le, puis envoyez-le au client. Pour remplir le formulaire, vous aurez besoin des informations suivantes:

    -   Les coordonnées du partenaire actuel et son ID Microsoft. Dans le menu de l’Espace partenaires, sélectionnez **Paramètres du compte** &gt; **Profil d’entreprise**, et utilisez les informations **ID Microsoft**, **Nom de l’organisation** et **Adresse** indiquées ici.

    -   L’IDMicrosoft du client. Dans le menu de l’Espace partenaires, sélectionnez **Clients**, puis développez la page de description du client pour voir son **IDMicrosoft**.

    -   L’ID d’abonnement à transférer. Dans la page de description développée du client, sélectionnez **Afficher les abonnements**, puis développez l’abonnement choisi pour voir son **ID d’abonnement**.

4.  Client et nouveau fournisseur de solutionsCloud de l’abonnement:

    Vérifiez le formulaire, renseignez les informations sur le nouveau partenaire, puis signez-le. Vérifiez que le nouveau client dispose d’un accord de contrat. Renvoyez le formulaire au partenaire de référence actuel.

    *Important*: si le nouveau partenaire Fournisseur de solutionsCloud n’a pas de relation de revendeur avec le client, il doit en établir une avant le transfert de l’abonnement. [Pour plus d’informations sur la marche à suivre, cliquez ici](https://int.msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

5.  Partenaire Fournisseur de solutionsCloud actuel:

    Vérifiez que le formulaire indique les coordonnées des deuxadministrateurs du partenaire. Le support Microsoft les contactera tous les deux pour confirmer le transfert. Assurez-vous que les trois signatures sont présentes et joignez le formulaire rempli à votre demande de service existante à l’aide de l’option **Chargement de fichier**. Un ingénieur du support Microsoft vous contactera sous 8heures ouvrées pour valider la réception et l’achèvement.

6.  Nouveau partenaire Fournisseur de solutionsCloud:

    Modifiez les paramètres d’abonnement Azure en supprimant l’ancien partenaire du compte. Pour afficher les attributions de rôle approvisionnées, exécutez deux applets de commande Powershell.

    -   Ajoutez le nouveau partenaire comme revendeur sur le compte:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        Pour trouver le customerDomainName: dans le menu de l’Espace partenaires, sélectionnez **Clients**. Dans la liste des clients, sélectionnez le client. Dans le menu client, sélectionnez **Compte** et utilisez le **Nom de domaine**.

    -   Affichez les rôles du compte, y compris les anciens partenaires Fournisseur de solutionsCloud:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

    Supprimez les autorisations obsolètes d’accès à l’abonnement et aux ressources en modifiant l’abonnement dans le portail Azure. Dans le menu de l’Espace partenaires, sélectionnez **Clients**. Développez la page de description et sélectionnez **Afficher les abonnements**. Dans le menu client, sélectionnez **Gestion des services**. Sous **MicrosoftAzure**, cliquez sur le lien pour accéder au **portail de gestion MicrosoftAzure**.

 

 






<!--HONumber=Nov16_HO4-->


