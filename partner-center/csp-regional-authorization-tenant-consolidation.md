---
title: "Consolidation des locataires disposant de l’autorisation régionale Fournisseur de solutions Cloud | Espace partenaires"
description: "Utilisez ces instructions pour consolider des locataires de différents pays/régions."
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 5d4b1acaa23f37df8fe66166f932956526e75271

---

# Consolidation des locataires disposant de l’autorisation régionale Fournisseur de solutionsCloud


\[Certaines informations concernent la version préliminaire de produits susceptibles d’être considérablement modifiés d’ici leur commercialisation. Microsoft ne donne aucune garantie, expresse ou implicite, concernant les informations fournies ici.\]

Utilisez ces instructions pour consolider des locataires de différents pays/régions.

**Remarque** Vous devez connaître tous les abonnements et le nombre de sièges de vos clients approvisionnés à partir des comptes de transition. Les partenaires réapprovisionneront ces mêmes abonnements avec le même nombre de sièges sous le nouveau compte central Fournisseur de solutionsCloud dans le cadre du processus de migration. Utilisez la fonctionnalité d’exportation de liste pour créer une liste de clients à transférer au locataire centralisé. Les partenaires choisissent de consolider leurs locataires. Une fois la consolidation terminée, les partenaires ne peuvent pas revenir à leur état antérieur. Notez qu’aucune action n’est requise de la part du client.

 

## Préparer la migration


-   Ouvrez une session sur <https://partnercenter.microsoft.com> avec le compte (existant) de transition et prenez note de tous les clients et de tous les services approvisionnés pour ces clients.

![liste de clients régionaux](images/regionalcustomer1.png)

## Migrer des comptes client


1.  Ouvrez une session sur <https://partnercenter.microsoft.com> avec le (nouveau) compte de transition et accédez à la liste de clients à partir du tableau de bord de l’Espace partenaires.

2.  Sélectionnez le client.

3.  Cliquez sur **Demander une relation de revendeur**. Un message électronique par défaut à présenter à vos clients s’affiche. Ce message contient une URL avec l’ID d’organisation propre à votre nouveau compte Espace partenaires.

4.  **Action du client:** vérifiez que chaque client actif que vous souhaitez migrer visite cette URL. À l’ouverture de l’URL, le client est invité à se connecter au portail Office365. Il se connecte à l’aide du même ID d’organisation que celui utilisé pour accéder aux portails administration Windows Azure et Office365.

5.  Une fois connecté, l’administrateur global du compte client est invité à valider l’attribution de privilèges d’administration délégué pour le nouveau compte Fournisseur de solutions Cloud. S’il accepte, le client active la case à cocher et autorise la relation.

Les clients s’affichent dans la liste des clients du partenaire, lorsqu’ils ont validé le présent contrat, un par un.

## Migration d’abonnements Office365 et non Azure basés sur l’utilisation


1.  Lorsque votre client a signé le contrat, vous pouvez recréer ses abonnements sous votre locataire partenaire centralisé.

2.  Dans le tableau de bord de l’Espace partenaires, cliquez sur **Clients** dans le panneau de navigation de gauche.

3.  Ouvrez le nom de la société du client que vous souhaitez migrer.

4.  Cliquez sur **Ajouter un abonnement**.

5.  Ajoutez les abonnements et le nombre de sièges corrects à partir du catalogue. Vérifiez avec les informations fournies dans les comptes de partenaire **Transition à partir de**.

    ![capture d’écran de la liste des clients](images/regionalcustomer2.png)

6.  Cliquez sur **Envoyer**.

Les services sont maintenant fournis au client à partir du compte de partenaire **Transition vers**.

Répétez ces étapes pour migrer les abonnements de tous les clients supplémentaires.

Avant de passer à la section suivante, vérifiez que tous les abonnements client existant sous les comptes de partenaire **Transition à partir de** sont ré-approvisionnées sous le compte de partenaire **Transition vers**.

**Remarque** Les partenaires doivent suspendre les abonnements sur le compte de locataire partenaire **Transition à partir de** dans l’Espace partenaires, le jour où ces abonnements sont transférés et configurés sous le compte de locataire partenaire **Transition vers** dans l’Espace partenaires pour éviter une double facturation. Les demandes de support seront refusées pour les crédits résultant d’un chevauchement dans la facturation à cause d’une désactivation incorrecte des abonnements **Transition à partir de**.

 

## Désactivation des abonnements Office365 sous le compte de partenaire Transition à partir de


La désactivation de l’abonnement Fournisseur de solutions Cloud sous les comptes de partenaire **Transition à partir de** interrompt toute facturation future. Il est inutile de désactiver manuellement les abonnements Azure, car le processus de migration les désactive automatiquement.

1.  Connectez-vous à <https://partnercenter.microsoft.com> avec le compte de Fournisseur de solutions Cloud **Transition à partir de** et accédez à la liste de clients.

2.  Ouvrez le client avec les abonnements à désactiver, et sélectionnez la première offre à désactiver.
3.  Réglez l’abonnement sur **suspendu**, puis cliquez sur **Envoyer**.

    **Remarque** La suspension de l’abonnement garantit l’absence de double facturation.

     

    L’abonnement affiche la mention **suspendu** dans la liste des abonnements.

4.  Répétez ces étapes pour tous les abonnements sous le client. Vérifiez que tous les abonnements indiquent la mention **suspendu**.

5.  Sélectionnez le client suivant sur la liste et répétez le processus de désactivation de tous les abonnements.

## Migration d’abonnements Azure basés sur l’utilisation


Notez qu’il est inutile de migrer manuellement les abonnements Fournisseur de solutions Cloud Azure basés sur l’utilisation, contrairement aux abonnements Fournisseur de solutions Cloud Office365. Le support Microsoft Azure peut migrer les abonnements Azure ainsi que tous les services ou ressources déployés entre les comptes de revendeur Fournisseur de solutions Cloud **Transition à partir de** et le compte de revendeur Fournisseur de solutions Cloud **Transition vers**. Il n’y a aucune interruption de service pour le client pendant cette transition.

1.  Vérifiez que les comptes client qui ont besoin d’abonnements Azure migrés ont accepté le contrat à associer au nouveau compte Fournisseur de solutions Cloud **Transition vers**.
2.  Les partenaires signalent à Microsoft que les comptes client qui ont des abonnements Azure sont prêts à migrer, et fournissent les noms de société de ces clients.
3.  Microsoft migre les abonnements Azure basés sur l’utilisation et avertit le partenaire lorsque la migration est terminée.
4.  Le partenaire confirme que l’abonnement Azure sous les comptes de revendeur Fournisseur de solutionsCloud **Transition à partir de** affiche la mention Suspendu dans l’Espace partenaires sous la section des abonnements du client.
5.  Le partenaire confirme que l’abonnement Azure sous le compte de revendeur Fournisseur de solutionsCloud **Transition à partir de** affiche la mention **Actif** dans l’Espace partenaires sous la section des abonnements du client.

    **Remarque** La désactivation des abonnements sous le client ne modifie pas l’apparence du client dans la liste de clients. Il n’y a actuellement aucune possibilité de supprimer des clients de la liste. Les partenaires doivent éviter de rajouter des abonnements à ces clients à partir de leur compte **Transition à partir de** à l’avenir.

     

6.  Répétez ces étapes pour tous les abonnements sous l’ensemble de vos clients pour arrêter les prochaines facturations sur le ou les comptes **Transition à partir de**. Le partenaire reçoit une facture finale avec un crédit pour le nombre de jours inutilisés entre le jour de l’annulation et le dernier jour de la période de facturation. Aucune facture n’est générée après cette période de facturation finale.

### Remarques

-   La désactivation de l’abonnement à partir du compte Fournisseur de solutionsCloud **Transition à partir de** n’affecte pas le service du client final, tant que le service est approvisionné à partir du compte Fournisseur de servicesCloud **Transition vers** avant la désactivation.

-   Le client ne peut pas utiliser les abonnements et ces derniers ne génèrent pas de frais en cas de suspension ou d’annulation.

-   Il est actuellement impossible de supprimer complètement un client de la liste de clients.

-   **Remarque** Les partenaires doivent suspendre les abonnements sur le compte de locataire partenaire **Transition à partir de** dans l’Espace partenaires, le jour où ces abonnements sont transférés et configurés sous le compte de locataire partenaire **Transition vers** dans l’Espace partenaires pour éviter une double facturation. Microsoft ne prend pas en charge les demandes de support pour les crédits résultant d’un chevauchement dans la facturation à cause d’une suspension incorrecte des abonnements **Transition à partir de**.

     

### Simplifier la migration avec l’exportation

Grâce à la **fonction Exporter**, vous pouvez capturer les abonnements que vous devez utiliser dans votre nouvelle structure consolidée:

1.  Cliquez sur **Clients** dans votre tableau de bord pour afficher la liste des clients dans votre structure existante.

2.  Ouvrez le nom de client souhaité.

3.  Dans la page **Abonnements**, cliquez sur **Exporter les abonnements** pour exporter les détails des abonnements dans un fichier Excel.

4.  Utilisez cette liste pour recréer les abonnements dans votre nouveau locataire consolidé.

### Inscription d’API

Pour plus d’informations sur l’inscription d’API, [consultez cette page](https://msdn.microsoft.com/en-us/library/partnercenter/mt267552.aspx).

## Journal d’activité de l’Espace partenaires


Avec le journal d’activité, les partenaires peuvent afficher un enregistrement de toutes les modifications apportées à leur locataire et qui affectent le client. Cela permet aux partenaires de suivre les modifications concernant un locataire du client.

**Afficher le journal d’activité**

1.  Dans le tableau de bord de l’Espace partenaires, cliquez sur le lien **Journal d’activité**.
2.  Dans la page **Journal d’activité**, affichez les modifications apportées aux comptes client. Pour filtrer le journal d’activité par date, renseignez les champs **de** et **à** afin de limiter le nombre d’enregistrements sélectionnés dans le journal. Pour effectuer un filtrage par client dans le **Journal d’activité**, utilisez la zone de recherche.

**Exporter le journal d’activité**

-   Cliquez sur **Exporter le journal** pour exporter les données de votre journal d’activité dans un fichierCSV.

    Vous pouvez également exporter la liste des clients et la liste des abonnements d’un client (à partir de la page des abonnements du client).

 

 






<!--HONumber=Nov16_HO4-->


