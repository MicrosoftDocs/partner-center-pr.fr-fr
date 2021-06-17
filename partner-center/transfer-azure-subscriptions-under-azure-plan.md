---
title: Transférer un abonnement Azure dans le cadre d’un plan Azure à un autre partenaire CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment modifier le partenaire du programme fournisseur de solutions Cloud associé aux abonnements Azure d’un client dans le cadre d’un plan Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 092c76fb874eb7308bdb69503223f722657db957
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277315"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Transférer les abonnements du plan Azure d’un client à un autre partenaire

**Rôles appropriés**: administrateur de compte | Agent commercial | Agent de facturation

Cet article décrit comment un client peut passer d’un fournisseur de solutions Cloud (CSP) à un autre dans le cadre d’un projet Azure.

Pour faire basculer les abonnements Azure d’un client d’un autre partenaire, procédez comme suit. Le partenaire et le client ont tous les deux la procédure à suivre.

>[!Note]  
>Seuls les partenaires disposant d’une relation de facturation directe avec Microsoft peuvent accéder aux outils de transition. Les revendeurs indirects doivent collaborer avec leurs fournisseurs indirects pour tirer parti de cet outil de transition.

Le client doit être en conversation avec les deux partenaires (actuels et futurs) avant de tirer parti de cet outil. Une conversation hors connexion doit être nécessaire pour éviter les confusions et les évolutions. En outre, les partenaires et les clients doivent comprendre ces considérations et conditions préalables avant d’initier une transition :

**Points clés :**

- Azure Reservations ne se déplacera pas avec l’abonnement au futur partenaire
- La tarification du fournisseur CSP pour les services Azure sous le partenaire actuel n’est pas transition  
- Les responsabilités de support pour le client seront déplacées vers le futur partenaire
- La facturation et la facturation seront déplacées vers le futur partenaire au moment du transfert
- Le Access Control de Role-Based Azure (RBAC) n’est pas affecté par le transfert
- L’administrateur pour le compte de (ADMINISTRATE) ne sera pas accordé par défaut au partenaire futur
- Les produits de la place de marché tiers sont transférés tant que les produits réussissent la vérification du droit de la place de marché.
    - Il n’existe aucune remise spéciale ou restriction régionale
    - Les produits ne sont pas basés sur un abonnement
    - Le futur partenaire devrait travailler avec le serveur de publication pour s’assurer qu’il se trouve dans la liste verte pour le déploiement du produit
    - Si certaines de ces conditions ne sont pas respectées pour transférer les produits de la place de marché, ils doivent être annulés, les abonnements Azure transférés, puis reacheter les produits de la place de marché auprès du nouveau partenaire.

**Configuration requise :**

- Le client fait appel au partenaire CSP actuel en cas de transition
- Le futur partenaire CSP travaille avec le client pour s’assurer que les besoins des clients peuvent être satisfaits
- Le futur partenaire CSP établit une relation avec le client et achète un plan Azure avant le début de la transition  
- Le client doit signer le contrat du client Microsoft avec un partenaire CSP futur
- Le futur partenaire CSP doit avoir signé l’accord de partenariat Microsoft pour utiliser cet outil

## <a name="customer-tasks-to-be-completed"></a>Tâches client à effectuer

Pour transférer un abonnement Azure dans le cadre d’un plan Azure, le client doit démarrer le processus en contactant son partenaire actuel. Ils doivent collecter le nom et le domaine de l’entreprise de leur partenaire actuel, de sorte que son partenaire futur puisse remplir le formulaire de demande de transfert en son nom.

Le client doit également identifier les abonnements qu’il souhaite transférer de son partenaire actuel. Vous ne pouvez pas changer de partenaire pour les abonnements Office 365, Enterprise Mobility suite ou Microsoft Dynamics CRM.

>[!Note]  
>Il incombe au futur partenaire de terminer le formulaire de demande de transfert qui initie le processus de transfert. Microsoft ne peut pas intervenir pour le compte du client ou du partenaire actuel. Le client doit planifier un travail en étroite collaboration avec son partenaire futur et actuel pour effectuer la transition en douceur.

## <a name="future-partner-tasks-to-be-completed"></a>Futures tâches de partenaire à effectuer

Le futur partenaire de l’abonnement doit remplir un formulaire de demande de transfert de l’espace partenaires pour demander un transfert d’abonnement :

1.  Dans le menu espace partenaires, sélectionnez **clients**, puis sélectionnez le client pour lequel vous souhaitez terminer un formulaire de demande de transfert pour le compte de.
2.  Dans le menu client, sélectionnez **abonnements**.
3.  Sélectionnez la section **demande de transfert** .
4.  Dans la **section demande de transfert**, sélectionnez **Ajouter une nouvelle demande**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Section des transferts.":::

5.  Complétez le formulaire **de demande de transfert** .

6.  Sélectionnez **Envoyer une demande de transfert**  >  **Envoyer**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Complétez le formulaire de demande de transfert.":::

7.  Vérifier la confirmation de demande de transfert

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Vérifiez le transfert en attente.":::

    >[!Note]
    >Le futur partenaire peut annuler la demande de transfert en sélectionnant **annuler la demande** dans le coin supérieur droit uniquement lorsque l’état de la demande de transfert est « en attente ». Une fois que l’état de la demande de transfert est « en cours » ou « terminé », les annulations ne sont pas possibles.

## <a name="current-partner-tasks-to-be-completed"></a>Tâches de partenaire actuelles à effectuer

L’agent admin du partenaire actuel recevra un e-mail indiquant que son client demande un transfert de ses abonnements :

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Révise.":::

Passez en revue et acceptez le formulaire de demande de transfert de l’espace partenaires pour terminer le transfert de l’abonnement.

>[!Note]  
>Si aucune action n’est effectuée par le partenaire actuel dans un délai de 30 jours, la demande expire et le partenaire futur aura un pour créer une demande de transfert.

1.  Sélectionnez **passer en revue la demande de transfert** à partir de l’e-mail ou
1.  Dans le menu espace partenaires, sélectionnez **clients**, puis sélectionnez le client pour lequel une demande de transfert a été soumise pour le compte de.
2.  Dans le menu client, sélectionnez **abonnements**.
3.  Sélectionnez la section **demande de transfert** .
4.  Développez les informations de transfert en sélectionnant l' **ID de demande de transfert** choisi sous **demandes reçues** .

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Demande de transfert de révisions de la source.":::

5.  Passez en revue la demande de transfert. Sélectionnez les abonnements Azure demandés à transférer.

>[!Note]  
> Avant de poursuivre, veuillez noter que vous n’aurez plus accès aux abonnements sélectionnés.
> Vous ne serez pas facturé pour une utilisation ultérieure.
> Les réservations Azure ne sont pas transférées avec les abonnements.

6.  Sélectionnez ensuite **accepter et transférer** pour terminer le processus de transfert.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Sélectionnez les abonnements à transférer sous vos plans Azure.":::

7.  Affichez la confirmation de l’acceptation du transfert.

   À ce stade, le futur partenaire, le client et le partenaire actuel seront avertis de la demande de transfert acceptée par courrier électronique.

   Après, la transition a été acceptée, l’état du transfert peut rester en attente pendant 15 minutes maximum pendant la mise à jour du système. Si cela prend plus de temps, le système continuera à essayer pendant trois jours. Si l’état du transfert reste toujours en attente, le partenaire doit soumettre une demande de service.

   Une fois le transfert terminé, les abonnements inclus dans la demande s’affichent dans le plan Azure du futur partenaire et ne sont plus répertoriés avec vous.

>[!Note]  
>Pour les fournisseurs indirects : Veuillez informer votre revendeur indirect que la demande de transfert a été acceptée.

### <a name="managing-your-transferred-customer-subscriptions"></a>Gestion de vos abonnements client transférés

- L’accès aux utilisateurs, groupes ou principaux de service existants auxquels a été affecté le contrôle d’accès en fonction du rôle Azure (RBAC) n’est pas affecté pendant la transition. Le contrôle d’accès en fonction du rôle [(RBAC)](/azure/role-based-access-control/overview) Azure permet à votre client de gérer qui a accès aux ressources Azure, ce qu’il peut faire avec ces ressources et les domaines auxquels ils ont accès. En tant que nouveau partenaire, vous ne disposez d’aucun accès RBAC aux ressources de votre client après le transfert de l’abonnement. Le partenaire précédent de votre client conserve son accès RBAC. Collaborez avec votre client pour comprendre qui a un aperçu de ses abonnements et comment apporter les modifications souhaitées.

- Par conséquent, il est important que votre client supprime l’accès RBAC Azure pour son partenaire précédent et ajoute un accès pour le nouveau partenaire. Pour plus d’informations sur votre client donnant accès à un nouvel accès, consultez [qu’est-ce que le contrôle d’accès en fonction du rôle Azure (Azure RBAC) ?](/azure/role-based-access-control/overview) Pour plus d’informations sur votre client qui supprime l’accès RBAC de votre partenaire précédent, consultez [supprimer une attribution de rôle](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- En outre, vous ne disposez pas automatiquement de l’accès de l’administrateur pour le [compte de (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) à vos abonnements. ADMINISTRATE est nécessaire pour que le partenaire gère les abonnements Azure de ses clients en leur nom. Pour plus d’informations sur les privilèges Azure, consultez [obtenir des autorisations pour gérer le service ou l’abonnement d’un client.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Étapes suivantes :

- [(RBAC Azure)](/azure/role-based-access-control/overview)
- [Obtenir des autorisations pour gérer le service ou l’abonnement d’un client.](./customers-revoke-admin-privileges.md)
