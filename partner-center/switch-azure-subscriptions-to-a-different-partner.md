---
title: Transférer un abonnement Azure à un autre partenaire
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment aider un client à modifier le partenaire du programme CSP associé aux abonnements Azure de ce client.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: LauraBrenner
ms.author: labrenne
keywords: abonnement Azure, changer de partenaire, changer de partenaire, acquérir un nouveau partenaire, autre partenaire
ms.custom: SEOMAY.20
ms.localizationpriority: medium
ms.openlocfilehash: eddab485d222bb8d0c5aae7cd977b6c85a418051
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425897"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Découvrez comment transférer les abonnements Azure d’un client à un autre partenaire

**S’applique à**

- Espace partenaires de Microsoft Cloud for US Government
- Espace partenaires pour Microsoft Global Cloud
- Partenaires du programme Fournisseur de solutions Cloud

Cet article décrit comment un client peut basculer ses services Microsoft Azure d’un fournisseur de solutions Cloud (CSP) vers un autre.

Pour faire basculer les services ou abonnements Azure d’un client vers un autre partenaire, suivez ces étapes manuelles. Le partenaire et le client doivent effectuer les étapes.

>[!Note]  
>Actuellement, seuls les fournisseurs directs ou indirects peuvent transférer des abonnements.
>Vous ne pouvez pas modifier les partenaires pour les abonnements de fournisseur de solutions Cloud associés aux abonnements Azure plan, Office 365, Enterprise Mobility suite ou Microsoft Dynamics CRM.

**Changer de partenaire pour les abonnements Azure**

1. Pour transférer un abonnement Azure à un nouveau partenaire, le client doit démarrer le processus et contacter son partenaire d’enregistrement en écriture.

   >[!Note]
   >Il incombe au partenaire actuel de créer le ticket de service qui initie le processus de transfert. Microsoft ne peut pas intervenir pour le compte du client ou du nouveau partenaire. Le client doit envisager de travailler en étroite collaboration avec le partenaire actuel pour effectuer la transition.

2. Le partenaire de l’abonnement doit effectuer les tâches suivantes :

   Créez un ticket de service Azure dans l’Espace partenaires pour demander un transfert d’abonnement&nbsp;:

   - Dans le menu espace partenaires, sélectionnez **clients**, sélectionnez votre client dans la liste, puis sélectionnez **gestion des services**. Dans la section **Tickets de support**, cliquez sur le menu déroulant **Nouveau ticket** et choisissez **Microsoft Azure**.

   - Dans le [portail Azure](https://portal.azure.com), sélectionnez **nouvelle demande de support**.

     À l’étape&nbsp;1, choisissez le type de problème **Gestion des abonnements**, indiquez l’ID d’abonnement que vous voulez transférer, puis choisissez **Fournisseur de solutions&nbsp;Cloud** comme formule d’assistance.

     À l’étape 2, sélectionnez **C-impact minimal** , puis choisissez **autres questions générales** comme type de problème.

     Téléchargez le [formulaire de transfert d’abonnement CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. Le partenaire de l’abonnement : Renseignez le [formulaire de transfert d’abonnement CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), signez-le, puis envoyez-le au client. Pour remplir le formulaire, vous aurez besoin des informations suivantes&nbsp;:

   - Les coordonnées du partenaire actuel et son ID Microsoft. Dans le menu de l’Espace partenaires, sélectionnez **Paramètres du compte** &gt; **Profil d’entreprise**, et utilisez les informations **ID Microsoft**, **Nom de l’organisation** et **Adresse** indiquées ici.

   - L’ID Microsoft du client. Dans le menu de l’Espace partenaires, sélectionnez **Clients**, puis développez la page de description du client pour voir son **ID&nbsp;Microsoft**.

   - L’ID d’abonnement à transférer. Dans la page de description développée du client, sélectionnez **Afficher les abonnements**, puis développez l’abonnement choisi pour voir son **ID d’abonnement**.

   >[!Note]
   >Le transfert d’un abonnement aboutit à deux ID d’abonnement que vous verrez dans la page **modifier l’abonnement** de l’abonnement transféré : **1**-l’ID d’abonnement du centre partenaires est utilisé à des fins de facturation. **2**-l’ID d’abonnement Azure d’origine est conservé et s’affiche dans l’espace partenaires, ainsi que dans le portail de gestion Azure. Cet ID s’affiche dans votre fichier de rapprochement.  **Lorsque la journalisation prend en charge les tickets, vous devez utiliser les deux ID.**

4. Le client et le nouveau partenaire pour l’abonnement :

   Vérifiez le formulaire, renseignez les informations sur le nouveau partenaire, puis signez-le. Vérifiez que le nouveau client dispose d’un accord de contrat. Renvoyez le formulaire au partenaire de référence actuel.

   *Important*: si le nouveau partenaire CSP n’a pas de relation de revendeur avec le client, il doit en établir un avant le transfert de l’abonnement. [Pour plus d’informations sur la marche à suivre, cliquez ici](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Le nouveau partenaire CSP et le locataire client doivent se trouver dans le même pays. 

5. Partenaire actuel :

   Assurez-vous que le formulaire contient des informations de contact pour les administrateurs du partenaire. Support Microsoft contacte les deux administrateurs pour vérifier le transfert. Vérifiez que vous disposez des trois signatures. Utilisez ensuite l’option de **chargement de fichier** pour attacher le formulaire terminé à votre demande de service existante. Un ingénieur du support technique Microsoft vous rappellera dans les huit heures ouvrables pour valider la réception et l’achèvement.

6. Nouveau partenaire :

   Modifiez les paramètres d’abonnement Azure en supprimant l’ancien partenaire du compte. Pour connaître les attributions de rôles approvisionnées, exécutez deux applets PowerShell.

   - Ajoutez le nouveau partenaire comme revendeur sur le compte :

     ```powershell
     Add-AzureRMAccount -tenant "CustomerDomainName"
     ```

     Pour trouver le customerDomainName : dans le menu de l’Espace partenaires, sélectionnez **Clients**. Dans la liste des clients, sélectionnez le client. Dans le menu client, sélectionnez **Compte** et utilisez le **Nom de domaine**.

   - Affichez les rôles du compte, y compris les anciens partenaires Fournisseur de solutions Cloud :

     ```powershell
     Get-AzureRMRoleAssignment
     ```

7. Supprimer les autorisations d’accès obsolètes

   - Dans le menu de l’Espace partenaires, sélectionnez **Clients**.
   - Développez la page de description et sélectionnez **Afficher les abonnements**.
   - Dans le menu client, sélectionnez **Gestion des services**.
   - Sous **Microsoft&nbsp;Azure**, cliquez sur le lien pour accéder au **portail de gestion Microsoft&nbsp;Azure**.
