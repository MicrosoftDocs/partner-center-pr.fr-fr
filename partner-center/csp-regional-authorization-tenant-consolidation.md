---
title: Consolidation des locataires disposant de l’autorisation régionale Fournisseur de solutions&nbsp;Cloud
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez ces instructions pour consolider des locataires de différents pays/régions. Cela comprend les étapes de migration des comptes client et des abonnements client.
author: LauraBrenner
ms.author: labrenne
keywords: migrer des clients, approvisionnement, compte de locataire, consolider les locataires
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2e3c0bd9b50e91e02952a690cc7cbfe1601ad550
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991470"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instructions pour le regroupement des locataires disposant de l’autorisation régionale CSP

**S’applique à**

-  Espace partenaires
-  Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Administrateur général
- Agent d’administration

\[Certaines informations relatives aux produits précommercialisés peuvent être substantiellement modifiées avant leur commercialisation. Microsoft exclut toute garantie, expresse ou implicite, concernant les informations fournies ici.\]

Utilisez ces instructions pour consolider des locataires de différents pays/régions.

>[!NOTE]  
>Vous devez être conscient de tous les abonnements et du nombre de sièges pour vos clients approvisionnés à partir des comptes de transition. Vous allez reconfigurer les mêmes abonnements exacts avec le même nombre de sièges sous le nouveau compte CSP central dans le cadre du processus de migration. Utilisez la fonctionnalité d’exportation de liste pour créer une liste de clients à transférer au locataire centralisé. Les partenaires choisissent de consolider leurs locataires. Une fois la consolidation terminée, les partenaires ne peuvent pas revenir à leur état antérieur. L’action du client peut également être nécessaire.

## <a name="prepare-for-migration"></a>Préparation de la migration

- Connectez-vous à l' **espace partenaires** avec le compte de **transition** (existant) (celui que vous allez passer) et passez en revue tous les clients et tous les services configurés pour ces clients.

   :::image type="content" source="images/regionalcustomer1.png" alt-text="liste de clients régionaux":::

## <a name="migrate-customer-accounts"></a>Migrer des comptes client

1. Connectez-vous à votre **espace partenaires** à l’aide du compte de **transition** (nouveau) (celui dans lequel vous effectuez la transition) et accédez à la liste Customers **(clients).**

2. Sélectionnez Clients.

3. Cliquez sur **Demander une relation de revendeur**. Un message électronique par défaut à présenter à vos clients s’affiche. Ce message contient une URL avec l’ID d’organisation propre à votre nouveau compte Espace partenaires.

4. **Action du client&nbsp;:** vérifiez que chaque client actif que vous souhaitez migrer visite cette URL. À l’ouverture de l’URL, le client est invité à se connecter au portail Office&nbsp;365. Il se connecte à l’aide du même ID d’organisation que celui utilisé pour accéder aux portails administration Windows Azure et Office&nbsp;365.

5. Une fois connecté, l’administrateur global du compte client est invité à valider l’attribution de privilèges d’administration délégué pour le nouveau compte Fournisseur de solutions Cloud. S’il accepte, le client active la case à cocher et autorise la relation.

Les clients s’affichent dans la liste des clients du partenaire après l’envoi de l’accord, un par un.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migration d’abonnements Office&nbsp;365 et non Azure basés sur l’utilisation

1. Lorsque votre client a signé le contrat, vous pouvez recréer ses abonnements sous votre locataire partenaire centralisé.

2. Dans l' **espace partenaires** , sélectionnez **clients**.

3. Ouvrez le nom de la société du client que vous souhaitez migrer.

4. Sélectionnez **Ajouter un abonnement**.

5. Ajoutez les abonnements et le nombre de sièges corrects à partir du catalogue. Vérifiez avec les informations fournies dans les comptes de partenaire **Transition à partir de**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Liste des clients":::

6. Cliquez sur **Envoyer.**

   Les services sont maintenant fournis au client à partir du compte de partenaire **Transition vers**.

7. Répétez ces étapes pour migrer les abonnements de tous les clients supplémentaires.

Avant de passer à la section suivante, vérifiez que tous les abonnements client existant sous les comptes de partenaire **Transition à partir de** sont ré-approvisionnées sous le compte de partenaire **Transition vers**.

> [!NOTE]
> Les partenaires doivent suspendre les abonnements lors de la transition **à partir du** compte de locataire partenaire dans l’espace partenaires le même jour que ces abonnements sont migrés et configurés dans le cadre du compte de locataire de partenaire dans l’espace partenaires pour s’assurer **que la double** facturation n’a pas lieu. Les demandes de support seront refusées pour les crédits résultant d’un chevauchement dans la facturation à cause d’une désactivation incorrecte des abonnements **Transition à partir de**.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Désactivation des abonnements Office&nbsp;365 sous le compte de partenaire Transition à partir de

La désactivation de l’abonnement Fournisseur de solutions Cloud sous les comptes de partenaire **Transition à partir de** interrompt toute facturation future. Il est inutile de désactiver manuellement les abonnements Azure, car le processus de migration les désactive automatiquement.

1. Connectez-vous à l' **espace partenaires** à l’aide de la **transition à partir du** compte CSP et accédez à la liste des clients.

2. Ouvrez le client avec les abonnements à désactiver, et sélectionnez la première offre à désactiver.

3. Réglez l’abonnement sur **suspendu**, puis cliquez sur **Envoyer**.

   >[!Note]
   >La suspension de l’abonnement garantit que la double facturation n’a pas lieu.

   L’abonnement affiche la mention **suspendu** dans la liste des abonnements.

4. Répétez ces étapes pour tous les abonnements sous le client. Vérifiez que tous les abonnements indiquent la mention **suspendu**.

5. Sélectionnez le client suivant sur la liste et répétez le processus de désactivation de tous les abonnements.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migration d’abonnements Azure basés sur l’utilisation

Azure, les abonnements CSP basés sur l’utilisation n’ont pas besoin d’être migrés manuellement comme c’est le cas avec les abonnements CSP Office 365. Le support Microsoft Azure peut migrer les abonnements Azure ainsi que tous les services ou ressources déployés entre les comptes de revendeur Fournisseur de solutions Cloud **Transition à partir de** et le compte de revendeur Fournisseur de solutions Cloud **Transition vers**. Il n’y a aucune interruption de service pour le client pendant cette transition.

1. Vérifiez que les comptes client qui ont besoin d’abonnements Azure migrés ont accepté le contrat à associer au nouveau compte Fournisseur de solutions Cloud **Transition vers**.

2. Les partenaires notifient à Microsoft les comptes client dont les abonnements Azure sont prêts à migrer, et fournit les noms de société de ces clients.

3. Microsoft migre les abonnements Azure basés sur l’utilisation et avertit le partenaire lorsque la migration est terminée.

4. Le partenaire confirme que l’abonnement Azure sous les comptes de revendeur Fournisseur de solutions&nbsp;Cloud **Transition à partir de** affiche la mention Suspendu dans l’Espace partenaires sous la section des abonnements du client.

5. Le partenaire confirme que l’abonnement Azure sous le compte de revendeur Fournisseur de solutions&nbsp;Cloud **Transition à partir de** affiche la mention **Actif** dans l’Espace partenaires sous la section des abonnements du client.

   >[!Note]
   > La désactivation des abonnements sous le client ne modifie pas l’apparence du client dans la liste des clients. Il n’y a actuellement aucune possibilité de supprimer des clients de la liste. Les partenaires doivent éviter de rajouter des abonnements à ces clients à partir de leur compte **Transition à partir de** à l’avenir.

6. Répétez ces étapes pour tous les abonnements sous l’ensemble de vos clients pour arrêter les prochaines facturations sur le ou les comptes **Transition à partir de**. Le partenaire reçoit une facture finale avec un crédit pour le nombre de jours inutilisés entre le jour de l’annulation et le dernier jour de la période de facturation. Aucune facture n’est générée après cette période de facturation finale.

### <a name="additional-information"></a>Informations supplémentaires

- La désactivation de l’abonnement de la **transition à partir** du compte CSP n’a pas d’impact sur le service du client final tant que le service a été approvisionné à partir du compte de **transition vers** le fournisseur CSP avant de désactiver l’abonnement.

- Les abonnements ne peuvent pas être utilisés par le client et ne génèrent pas de frais lorsqu’ils sont suspendus ou annulés.

- Il est actuellement impossible de supprimer complètement un client de la liste de clients.

    >[!Note]
    > Les partenaires doivent suspendre les abonnements lors de la transition à **partir du** compte de locataire partenaire dans l’espace partenaires le même jour auquel ces abonnements sont migrés et configurés dans le cadre du compte de locataire de partenaire dans l’espace partenaires pour s’assurer **que la double** facturation n’a pas lieu. Microsoft ne prend pas en charge les demandes de crédits en raison d’un chevauchement de la facturation qui résulte de la définition incorrecte du **passage des** abonnements à l’état suspendu.

### <a name="simplify-migration-using-export"></a>Simplifier la migration avec l’exportation

Grâce à la **fonction Exporter**, vous pouvez capturer les abonnements que vous devez utiliser dans votre nouvelle structure consolidée&nbsp;:

1. Cliquez sur **clients** dans l’espace partenaires pour afficher la liste des clients dans votre structure existante.

2. Ouvrez le nom de client souhaité.

3. Dans la page **Abonnements**, cliquez sur **Exporter les abonnements** pour exporter les détails des abonnements dans un fichier Excel.

4. Utilisez cette liste pour recréer les abonnements dans votre nouveau locataire consolidé.

### <a name="api-registration"></a>Inscription d’API

Pour plus d’informations sur l’inscription d’API, consultez [configurer l’accès aux API dans l’espace partenaires](https://go.microsoft.com/fwlink/?linkid=847990).
