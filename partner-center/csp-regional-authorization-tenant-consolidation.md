---
title: Consolidation des locataires disposant de l’autorisation régionale Fournisseur de solutions&nbsp;Cloud
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez ces instructions pour consolider des locataires de différents pays/régions. Cela comprend les étapes de migration des comptes client et des abonnements client.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502568"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instructions pour le regroupement des locataires disposant de l’autorisation régionale CSP

**S’applique à**

- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Administrateur général
- Agent d’administration

\[Certaines informations relatives aux produits précommercialisés peuvent être substantiellement modifiées avant leur commercialisation. Microsoft ne donne aucune garantie, expresse ou implicite, concernant les informations fournies ici.\]

Vous pouvez consolider les locataires pour votre entreprise. Utilisez ces instructions pour consolider des locataires de différents pays/régions.

>[!NOTE]  
>Vous devez être conscient de tous les abonnements approvisionnés et du nombre de licences pour chacun de vos clients dans le compte à partir duquel vous effectuez la transition. Vous allez reconfigurer les mêmes abonnements exacts avec le même nombre de licences sous le nouveau compte CSP central dans le cadre du processus de migration. Utilisez la fonctionnalité d’exportation de liste pour créer une liste de clients à transférer au locataire centralisé.  Une fois la consolidation terminée, vous ne pouvez pas revenir à l’état précédent du locataire. L’action du client peut également être nécessaire.

## <a name="prepare-for-migration"></a>Préparation de la migration

- Connectez-vous à l' **espace partenaires**  à l’aide du compte de **transition** (celui que vous allez migrer vers le nouveau compte) et passez en revue tous les clients et tous les services approvisionnés pour ces clients.

- Déconnectez-vous de ce compte.

## <a name="migrate-customer-accounts"></a>Migrer des comptes client

1. Connectez-vous à l' **espace partenaires**  avec le compte de **transition** (nouveau) (celui vers lequel vous transférez des clients).

2. Sélectionnez **Clients**.

3. Sélectionnez **demander une relation de revendeur**. Vous êtes invité à envoyer un message électronique par défaut à vos clients. Ce message contient une URL avec l’ID d’organisation propre à votre nouveau compte Espace partenaires.

4. **Action du client&nbsp;:** vérifiez que chaque client actif que vous souhaitez migrer visite cette URL. À l’ouverture de l’URL, le client est invité à se connecter au portail Office&nbsp;365. Il se connecte à l’aide du même ID d’organisation que celui utilisé pour accéder aux portails administration Windows Azure et Office&nbsp;365.

5. Une fois connecté, l’administrateur général du **compte client** est invité à soumettre un accord qui accorde des privilèges d’administrateur délégué au nouveau compte CSP. S’il accepte, le client active la case à cocher et autorise la relation.

Les clients s’affichent dans la liste des clients du partenaire après l’envoi de l’accord, un par un.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migration d’abonnements Office&nbsp;365 et non Azure basés sur l’utilisation

1. Lorsque votre client a signé le contrat, vous pouvez recréer ses abonnements sous votre locataire partenaire centralisé.

2. Dans l' **espace partenaires**, sélectionnez **clients**.

3. Ouvrez le nom de la société du client que vous souhaitez migrer.

4. Sélectionnez **Ajouter un abonnement**.

5. Ajoutez les abonnements et le nombre de licences appropriés à partir du catalogue. Vérifiez avec les informations fournies dans les comptes de partenaire **Transition à partir de**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Liste des clients":::

6. Sélectionnez **Envoyer.**

   Les services sont maintenant fournis au client à partir du compte de partenaire **Transition vers**.

7. Répétez ces étapes pour migrer les abonnements de tous les clients supplémentaires.

Avant de passer à la section suivante, vérifiez que tous les abonnements client existant sous les comptes de partenaire **Transition à partir de** sont ré-approvisionnées sous le compte de partenaire **Transition vers**.

> [!NOTE]
> Les partenaires doivent suspendre les abonnements lors de la transition **à partir du** compte de locataire partenaire dans l’espace partenaires le même jour que ces abonnements sont migrés et configurés dans le cadre du compte de locataire de partenaire dans l’espace partenaires pour s’assurer **que la double** facturation n’a pas lieu. Les demandes de support sont refusées pour les crédits en raison du chevauchement de la facturation résultant de la désactivation incorrecte **de la transition des** abonnements.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Désactivation des abonnements Office&nbsp;365 sous le compte de partenaire Transition à partir de

La désactivation de l’abonnement Fournisseur de solutions Cloud sous les comptes de partenaire **Transition à partir de** interrompt toute facturation future. Vous n’avez pas besoin de désactiver manuellement les abonnements Azure, car les abonnements Azure sont automatiquement désactivés pendant le processus de migration.

1. Connectez-vous à l' **espace partenaires** à l’aide de la **transition à partir du** compte CSP et accédez à la liste des clients.

2. Ouvrez le client avec les abonnements à désactiver, et sélectionnez la première offre à désactiver.

3. Définissez l’abonnement sur **suspendu**, puis sélectionnez **Envoyer**.

   >[!Note]
   >La suspension de l’abonnement garantit que la double facturation n’a pas lieu.

   L’abonnement affiche **suspendu** dans la liste des abonnements.

4. Répétez ces étapes pour tous les abonnements sous le client. Vérifiez que tous les abonnements indiquent la mention **suspendu**.

5. Sélectionnez le client suivant sur la liste et répétez le processus de désactivation de tous les abonnements.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migration d’abonnements Azure basés sur l’utilisation

Contrairement aux abonnements CSP Office 365, Azure, les abonnements CSP basés sur l’utilisation n’ont pas besoin d’être migrés manuellement. Microsoft Azure prise en charge migre les abonnements Azure et tous les services ou ressources déployés de la **transition des** comptes du revendeur CSP vers le compte du revendeur de la **transition vers** le revendeur CSP. Il n’y a aucune interruption de service pour le client pendant cette transition.

1. Assurez-vous que les comptes clients pour lesquels des abonnements Azure ont été migrés ont accepté le contrat à associer à la nouvelle **transition vers** le compte CSP.

2. Vous informerez Microsoft des comptes client prêts à migrer et fournissez les noms de société de ces clients.

3. Microsoft migre les abonnements basés sur l’utilisation d’Azure et vous avertit lorsque la migration est terminée.

4. Vous devez vérifier que l’abonnement Azure sous le compte **de** revendeur du revendeur CSP est désormais marqué comme **suspendu** dans l’espace partenaires dans la section abonnements client.

5. Confirmez que l’abonnement Azure sous le compte du revendeur **de la transition au** revendeur CSP affiche maintenant l’état **actif** dans l’espace partenaires dans la section abonnements client.

   >[!Note]
   > La désactivation des abonnements sous le client ne modifie pas l’apparence du client dans la liste des clients. Il n’y a actuellement aucune possibilité de supprimer des clients de la liste. Les partenaires doivent éviter de rajouter des abonnements à ces clients à partir de leur compte **Transition à partir de** à l’avenir.

6. Répétez ces étapes pour tous les abonnements sous l’ensemble de vos clients pour arrêter les prochaines facturations sur le ou les comptes **Transition à partir de**. Le partenaire reçoit une facture finale avec un crédit pour le nombre de jours inutilisés entre le jour de l’annulation et le dernier jour de la période de facturation. Aucune facture n’est générée après cette période de facturation finale.

### <a name="additional-information"></a>Informations supplémentaires

- La désactivation de l’abonnement de la **transition à partir** du compte CSP n’a pas d’impact sur le service du client final tant que le service a été approvisionné à partir du compte de **transition vers** le fournisseur CSP avant de désactiver l’abonnement.

- Les abonnements ne peuvent pas être utilisés par le client et ne génèrent pas de frais lorsqu’ils sont suspendus ou annulés.

- Il n’existe actuellement aucun moyen de supprimer complètement un client de la liste des **clients** .
- 
    >[!Note]
    > Les partenaires doivent suspendre les abonnements lors de la transition à **partir du** compte de locataire partenaire dans l’espace partenaires le même jour que celui vers lequel les abonnements sont migrés et configurés sous le compte de **transition** pour s’assurer que la double facturation n’a pas lieu. Microsoft ne prend pas en charge les demandes de crédits en raison d’un chevauchement de la facturation qui résulte de la définition incorrecte du **passage des** abonnements à l’état suspendu.

### <a name="simplify-migration-using-export"></a>Simplifier la migration avec l’exportation

Grâce à la **fonction Exporter**, vous pouvez capturer les abonnements que vous devez utiliser dans votre nouvelle structure consolidée&nbsp;:

1. Sélectionnez **clients** dans l’espace partenaires pour afficher la liste des clients. 

2. Ouvrez le nom de client souhaité.

3. Sur la page **abonnements** , sélectionnez **Exporter les abonnements** pour exporter les détails des abonnements vers un fichier Excel.

4. Utilisez cette liste pour recréer les abonnements dans votre nouveau locataire consolidé.

### <a name="api-registration"></a>Inscription d’API

Pour plus d’informations sur l’inscription d’API, consultez [configurer l’accès aux API dans l’espace partenaires](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Étapes suivantes

- [Les marchés régionaux et les devises du programme fournisseur de solutions Cloud dans lesquels vous pouvez vendre des offres CSP](regional-authorization-overview.md)
