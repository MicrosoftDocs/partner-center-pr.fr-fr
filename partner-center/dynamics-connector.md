---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisation du connecteur Dynamics 365 pour recevoir des références de Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: bddd29e9136d998ef8a25616d2058d1380b36665
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825686"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble

### <a name="appropriate-roles"></a>Rôles appropriés

- Administrateur des références
- Administrateur système ou personnalisateur de système sur le CRM

Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM. Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente. À l’aide des connecteurs de covente, vous serez en mesure de créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de transaction, telles que la valeur de la transaction, la date de clôture, etc., ainsi que recevoir les mises à jour des vendeurs Microsoft sur ces offres de covente Vous pouvez effectuer toutes ces tâches tout en travaillant dans le CRM de votre choix plutôt que dans l’espace partenaires. 

La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires Microsoft.

## <a name="before-you-install---pre-requisites"></a>Avant d’installer-conditions préalables

|**Rubriques**   |**Détails**   |**Liens**   |
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Vous avez besoin d’un ID MPN valide|Pour rejoindre [MPN](https://partner.microsoft.com/)|
|Co-vente prête|Votre solution IP/Services doit être prête à être covente.|[Vendre avec Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Compte Espace partenaires|L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente. Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.|[Gérer votre compte](create-user-accounts-and-set-permissions.md)|
|Rôles d’utilisateur de l’Espace partenaires|L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références|[Affecter des rôles et des autorisations aux utilisateurs](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système|[Affecter des rôles dans Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Gestion de l’alimentation-automatiser le compte|Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM. Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate) 

1. Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit. Les instances CRM disponibles s’affichent.

2. Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit. 

3. Sélectionnez **solutions** dans la barre de navigation de gauche.

4. Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.

![Ouvrir AppSource](images/cosellconnectors/openappsource.png)

5. Recherchez les **connecteurs de références de l’espace partenaires pour Dynamics365** dans l’écran contextuel.  

6. Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**. 

7. Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.  Acceptez les conditions générales. 

8. Vous êtes ensuite dirigé vers la page **gérer vos solutions** .  Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page. **L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires. L’installation prendra 10-15 minutes. 

9. Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche. Notez que la **synchronisation des références de l’espace partenaires pour Dynamics 365** est disponible dans la liste des solutions.

10. Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**. Les flux et entités Power automate suivants sont disponibles :

![CRM disponibles](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>Meilleure pratique : testez avant de passer en direct

Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.

- Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.
- Effectuez une copie de la solution et effectuez votre configuration et automatisez les personnalisations de flow sur l’environnement intermédiaire.
- Testez la solution sur une instance intermédiaire/CRM. 
- En cas de réussite, importez en tant que solution gérée dans l’instance de production. 

## <a name="configure-the-solution"></a>Configurer la solution

1. Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).

2. Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.

3. Vous devrez créer des connexions qui associent les trois comptes d’utilisateur : 

- Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références 
- Événements de l’Espace partenaires
- L’administrateur CRM avec les flux Power automate dans la solution. 

    a. Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.
    b. Créez une connexion en cliquant sur **créer une connexion**. 

    ![Créer une connexion](images/cosellconnectors/createconnection.png)
    
    c. Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.
    d. Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références. Envoyer. Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références. FA. Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.

4. Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires. Enregistrez les modifications.

5. **Activez** les flux automate Power.

## <a name="next-steps"></a>Étapes suivantes

- [Utiliser des webhooks pour recevoir des événements de modification de ressource](referral-connector-webhooks.md)

- [En savoir plus sur la plateforme Microsoft Power Automated ?](https://docs.microsoft.com/power-automate/)

- [Gérer les prospects](manage-leads.md)

- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)

