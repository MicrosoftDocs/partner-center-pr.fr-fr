---
title: Gérer les licences dans les offres de la place de marché
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment configurer et gérer les licences pour vos offres de la place de marché ISV commercial.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284871"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Gérer les licences dans les offres de la place de marché

**Rôles appropriés**

- Administrateur général
- Administrateur des comptes

Cet article vous guide tout au long du processus de configuration d’une offre dans l’espace partenaires, de sa mise à disposition dans Microsoft AppSource, puis de la gestion des licences pour cette offre.  

>[!IMPORTANT]
>Les fonctionnalités de cet article sont actuellement en version préliminaire publique.

## <a name="before-you-begin"></a>Avant de commencer

Avant de commencer ce processus, vous devez vous familiariser avec les informations ci-dessous.

### <a name="review-the-azure-marketplace-documentation"></a>Consulter la documentation de la place de marché Azure

Les articles ci-dessous contiennent des informations que vous devez connaître avant de continuer. 

- [Créer une offre Dynamics 365 for Customer Engagement et PowerApps](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [Créer un compte Place de marché commerciale dans l’Espace partenaires](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a>Créer votre ID d’offre

Dans les procédures ci-dessous, vous serez invité à entrer un ID d’offre. Prenez le temps de trouver un ID d’offre approprié, en gardant à l’esprit les points suivants :

- Cet ID est visible par les clients dans l’adresse web de l’offre de la Place de marché et des modèles Resource Manager, le cas échéant.
- L’ID d’offre associé à l’ID d’éditeur doit contenir moins de 40 caractères.
- Utilisez uniquement des lettres minuscules et des chiffres. L’ID de l’offre peut inclure des traits d’Union et des traits de soulignement, mais aucun espace. Par exemple, si votre ID d’éditeur est testpublisherid et que vous entrez test-offer-1, l’adresse Web de l’offre sera https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .
- Cet ID ne peut pas être changé une fois que vous avez sélectionné **Créer**.

### <a name="create-your-offer-alias"></a>Créer votre alias d’offre

L’alias d’offre est le nom utilisé pour l’offre dans l’espace partenaires. Vous aurez également besoin d’un alias d’offre approprié qui respecte les instructions ci-dessous :

- Ce nom n’est pas utilisé dans la Place de marché et est différent du nom de l’offre et des autres informations présentées aux clients.
- Ce nom ne peut pas être modifié après que vous ayez sélectionné Créer.

## <a name="create-your-offer"></a>Créer votre offre

La première étape du processus de gestion des licences consiste à créer votre offre de la place de marché commercial. 

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).
2. Dans le menu de navigation de gauche, sélectionnez **Marketplace commercial/vue d’ensemble**.
3. En haut de la page vue d’ensemble, sélectionnez **nouvelle offre**, puis sélectionnez **Dynamics 365 pour engagement client & powerapps**.
4. Entrez l' **ID d’offre** et l' **alias d’offre** que vous avez créés précédemment.
5. Sélectionnez **Créer** pour générer l’offre et continuer.
6. Choisissez vos options de licence.

    - Pour activer la gestion des licences pour votre offre, sélectionnez **activer la gestion des licences d’application par le biais de Microsoft**. Il s’agit d’un paramètre unique, et vous ne pouvez pas le modifier une fois que votre offre est publiée.

    - Vous pouvez également permettre aux clients d’exécuter les fonctionnalités de base de votre application sans licence, et d’exécuter des fonctionnalités Premium une fois qu’elles ont acheté une licence. Pour ce faire, sélectionnez **autoriser les clients à installer mon application même si les licences ne sont pas attribuées**.

    - Si vous ne souhaitez pas que votre offre soit activée pour la gestion des licences, sélectionnez **obtenir maintenant (gratuit)**, **version d’évaluation gratuite** ou **Contactez-moi**.

## <a name="create-your-plan"></a>Créer votre plan

Dans ces étapes, vous allez définir les plans que vous souhaitez activer pour votre offre.

1. Dans le menu de navigation de gauche, sélectionnez **vue d’ensemble du plan**, puis sélectionnez **créer un plan**.
2. Entrez un **ID de plan** et un **nom de plan**, puis sélectionnez **créer**.
3. Dans la page **liste des plans** , entrez la description de votre **plan**.
4. Pour enregistrer la description et terminer ultérieurement, sélectionnez **Enregistrer brouillon**.

5. Lorsque vous avez terminé, sélectionnez **examiner et publier**. Les informations sur le plan s’affichent désormais sur appsource.microsoft.com sous liste des offres (section plans).

6. Une fois que vous avez créé tous les plans de cette offre, vous devez copier l’ID de service de chaque plan. Sélectionnez **vue d’ensemble du plan** en haut de la page de liste des plans. Copiez l’ID de service de chaque plan dans un emplacement sûr.

## <a name="add-service-ids-to-your-solution"></a>Ajouter des ID de service à votre solution

L’étape suivante consiste à mettre à jour votre solution en ajoutant les ID de service pour chaque plan que vous venez de copier. Pour obtenir de l’aide, consultez [créer un package AppSource pour votre solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).

## <a name="upload-your-package-and-publish-your-offer"></a>Télécharger votre package et publier votre offre

1. Dans le volet de navigation gauche, sélectionnez **commercial Marketplace**, puis sélectionnez **configuration technique**.
2. Sous **modèle de licence de base**, sélectionnez **utilisateur**.
3. Sous **package CRM**, entrez l’URL de l’emplacement de votre package.
4. Utilisez les autres onglets du volet de navigation gauche pour entrer les autres informations requises. Lorsque vous avez terminé, sélectionnez **examiner et publier**.

Une fois l’offre publiée, nous examinerons et vérifierons vos informations. En cas de problème avec ce processus, nous vous en informerons. Lorsque tous les problèmes ont été résolus, vous recevez une notification vous informant que votre offre est disponible dans AppSource. À ce stade, vous pouvez le rendre actif.

## <a name="make-your-offer-live-in-partner-center"></a>Rendre votre offre active dans l’espace partenaires

La procédure suivante vous guide tout au long du processus de mise en production de votre offre dans AppSource. Pour en savoir plus sur ce processus, consultez [Présentation des options de liste](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).

>[!NOTE]
>Une fois que vous avez publié votre offre, le temps de mise en ligne est de 4-6 heures.

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).
2. Dans le menu de navigation de gauche, sélectionnez **Marketplace commercial/vue d’ensemble**.
3. Sur la page **vue d’ensemble** , recherchez l’offre que vous recherchez. Les offres prêtes à être publiées auront l’État version **préliminaire**. Sélectionnez l’offre.
4. Sur la page **vue d’ensemble** de l’offre, sélectionnez **Go Live**.
L’offre sera en ligne dans 4-6 heures.
5. Pour afficher la liste de vos offres sur AppSource, sélectionnez le lien **AppSource** au bas de la page **vue d’ensemble** de l’offre.

    - **Pour les offres avec licence**: Si votre offre requiert une vérification de licence, les utilisateurs pourront uniquement entrer un prospect en cliquant sur **me contacter** pour vous permettre de communiquer avec eux.

    - **Pour les offres avec licence activée avec l’option d’installation gratuite**: Si votre offre ne nécessite pas de vérification de licence, les utilisateurs administrateurs verront s’afficher un bouton **obtenir maintenant** en plus de **me contacter**. Les utilisateurs qui souhaitent essayer votre option d’installation gratuite doivent cliquer sur **obtenir maintenant**, ce qui leur permet d’installer l’offre sur le centre d’administration Power Platform. Les utilisateurs peuvent toujours utiliser **me contacter** s’ils ont des questions ou s’ils souhaitent effectuer une mise à niveau vers un plan payant.

## <a name="register-isv-connect-deal-in-dealreg"></a>Inscrire la transaction ISV Connect dans DealReg

L’étape suivante consiste à inscrire votre contrat. Pour ce faire, consultez [inscrire vos demandes](https://docs.microsoft.com/partner-center/register-deals).

## <a name="invite-the-customer"></a>Inviter le client

Utilisez la procédure suivante pour inviter le client à participer à cette transaction.  

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).
2. Dans le menu de navigation de gauche, sélectionnez **Marketplace commercial/vue d’ensemble**.
3. Filtre pour les demandes **envoyées** , sélectionnez l’onglet **en cours** , puis sélectionnez le contrat que vous souhaitez.
4. Dans la page vue d’ensemble de cette offre, sélectionnez **gérer les licences**.
5. Dans la fenêtre **gérer les licences** , sélectionnez le client dans la liste déroulante Détails du **client** . Si la relation client n’existe pas encore, sélectionnez **+ inviter un nouveau client à donner son consentement**.
6. Copiez le lien qui s’affiche.
7. Envoyez ce lien par courrier électronique à l’administrateur général ou à l’administrateur de facturation de votre client, et demandez-lui d’utiliser ce lien pour accéder à admin.microsoft.com et pour accepter et autoriser la relation que vous établissez.

    >[!NOTE]
    >La relation ne sera pas établie tant que le client n’aura pas effectué cette étape.

## <a name="activate-manage-and-remove-your-licenses"></a>Activer, gérer et supprimer vos licences

Une fois votre client établi, vous pouvez commencer à ajouter des plans à partir de votre offre et affecter des licences à chaque plan.

1. Dans la fenêtre gérer les licences pour cette offre, sélectionnez **+ Ajouter un plan**.
2. Complétez les champs **plans pour cette solution** et **nombre de licences** , puis sélectionnez **mettre à jour les licences**. Les licences seront disponibles sur admin.microsoft.com pour que les clients puissent les gérer et les affecter aux employés.

    - Pour modifier le nombre de licences pour un plan existant, entrez le nouveau nombre dans le champ **nombre de licences** , puis sélectionnez **mettre à jour les licences**.

    - Pour désactiver ou supprimer des licences pour un contrat, sélectionnez l’icône de la corbeille dans le champ **actions** , puis sélectionnez **mettre à jour les licences**.