---
title: Comment acheter une offre SaaS dans Portail Azure
description: Découvrez comment rechercher et acheter une offre SaaS dans Portail Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: 8dba9f95607a4172e6d5d0bc2ec148a25b599cd1
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431449"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Acheter une offre SaaS dans Portail Azure

Cet article explique les différentes options et exigences relatives à la recherche, à l’essai et à l’achat d’une offre SaaS (Software-as-a-service) à partir de la Portail Azure.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS offre une découverte dans Portail Azure

Une fois que vous êtes en Portail Azure, vous pouvez affiner votre recherche pour vous concentrer sur les offres SaaS.

### <a name="narrowing-your-search"></a>Affiner votre recherche

Sur la page d’accueil, sous **services Azure** , sélectionnez **+ créer une ressource ou une place de** **marché**. Ou utilisez le raccourci **G + N** n’importe où dans la plateforme.

- Réduisez les résultats aux offres SaaS à l’aide du filtre **type d’offre** , puis sélectionnez **Saas**.
- Utilisez la barre de recherche globale située dans la zone de navigation supérieure pour rechercher une offre SaaS spécifique.

Recherchez une [offre SaaS privée](/marketplace/private-offers) en sélectionnant la bannière en haut de la page d’accueil de la place de **marché** . Toutes les offres, ou les plans ne sont pas disponibles dans toutes les zones géographiques et certains peuvent uniquement apparaître pour certains locataires.

La vue filtrée affiche chaque offre SaaS disponible représentée par un titre. Sélectionnez-en un pour afficher la page Détails du produit. Qui comprend les sections suivantes :

- Vue d’ensemble : détails sur le service, le marketing et les supports de formation
- Plans + tarification : chaque offre inclut au moins un plan avec des conditions de facturation et des prix différents
- Informations d’utilisation + support : comprend l’ID de l’éditeur, l’ID de l’offre et l’ID du plan
- Évaluation et évaluations de l’offre SaaS spécifique

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modèles de facturation disponibles (plans/références SKU) pour les offres SaaS

Chaque offre SaaS aura un ou plusieurs plans. Chaque offre est associée à un modèle de tarification : forfaitaire ou par utilisateur. Chaque prix de plan est payant, ce qui peut être égal à zéro dollar (les prix répertoriés sont fournis à titre d’exemple uniquement et ne sont pas destinés à refléter les coûts réels). Ces frais sont soit forfaitaires, soit tarif par utilisateur. Types de plans disponibles :

- **Plans mensuels** – frais mensuels périodiques ; frais mensuels fixes ou par utilisateur payés sur une périodicité mensuelle. Une fois le terme terminé, le plan est renouvelé automatiquement.
- **Plans annuels** – frais annuels périodiques ; frais annuels forfaitaires ou par utilisateur payés sur une récurrence annuelle. Une fois le terme terminé, le plan est renouvelé automatiquement.
- **Compteurs personnalisés** : en plus des frais récurrents, un plan forfaitaire peut également inclure des dimensions limitées facultatives pour l’utilisation de dépassement non incluses dans le tarif forfaitaire. Chaque dimension représente une unité facturable. Il s’agit d’un coût variable qui change en fonction de l’utilisation d’unités limitées, telles que la bande passante, les tickets ou le courrier électronique traité. Vous serez facturé en fonction de votre consommation de ces dimensions sur une base mensuelle. Notez que la consommation de dépassement commence uniquement lorsque vous avez utilisé toutes les unités limitées incluses dans le tarif fixe.
- **Essai gratuit** : dans certains cas, le plan comprend une période d’essai d’un mois, pendant laquelle vous pouvez utiliser le logiciel gratuitement.  Une fois la période d’essai terminée, vous serez facturé en fonction de votre plan. Les offres d’essai ne sont pas compatibles avec les compteurs personnalisés.

Ces modèles de tarification sont disponibles pour les plans publics et privés.

## <a name="saas-purchase-experience"></a>Expérience d’achat SaaS

1. Sur la page du produit, sélectionnez un plan qui répond à vos besoins et continuez à **configurer + s’abonner**
2. Dans le cadre du processus d’achat, vous êtes redirigé vers l’onglet de **base** et vous êtes invité à :
    1. Définissez l' *abonnement* que vous souhaitez utiliser pour la facturation. L’abonnement Azure que vous utilisez doit avoir une méthode d’achat valide définie. Vous devez disposer du niveau d’autorisation approprié ou avoir un groupe de ressources sous cet abonnement avec le niveau d’autorisations approprié. En outre, son pays de facturation doit être un pays dans lequel l’offre est disponible à l’achat. Les abonnements Azure sans mode de paiement valide (par exemple, un abonnement MSDN) peuvent uniquement être utilisés pour acheter des plans gratuits
    1. Choisissez ou créez un *groupe de ressources* * auquel appartiendra la ressource Saas.
    1. Tapez un *nom* pour l’abonnement SaaS pour l’identifier facilement ultérieurement. Une fois acheté, vous ne pouvez plus modifier le nom.
    1. Sous **plan**, vous verrez le plan que vous avez sélectionné dans la page de détails du produit (PDP). Si vous n’avez pas effectué de sélection active dans le PDP, vous verrez le plan par défaut. Vous pouvez modifier votre sélection en sélectionnant le lien **modifier le plan** . Sélectionnez le terme de facturation approprié, puis choisissez un autre plan. Vous pourrez peut-être modifier le plan après l’achat si le serveur de publication le prend en charge. Toutefois, vous ne serez pas en mesure de changer le terme mensuel en année ou annuel en mensuel.
    1. Dans les cas où le modèle de tarification est *par utilisateur*, vous pouvez être amené à spécifier le nombre d' *utilisateurs*. Le prix que vous voyez change en fonction de l’abonnement, du plan et du terme que vous avez sélectionnés.
3. Passer à l’onglet **balises** : les *balises* sont des paires clé/valeur définies par l’utilisateur, qui peuvent être placées directement sur une ressource ou un groupe de ressources. Vous pouvez utiliser des balises pour retrouver facilement votre ressource SaaS plus tard. Azure prend actuellement en charge jusqu’à 50 étiquettes par ressource et par groupe de ressources. Les balises peuvent être placées sur une ressource au moment de la création ou bien ajoutées à une ressource existante.
4. Passez à l' **examen + abonnement** pour parcourir les détails de l’offre et du plan.
    1. Passer en revue les *conditions d’utilisation*, les *modifications* et la *politique de confidentialité* du serveur de publication et de la place de marché Azure
    1. Vous pouvez être invité à ajouter vos coordonnées
    1. Examiner les *concepts de base* et les détails des *étiquettes*
5. Après confirmation, sélectionnez **s’abonner**.

## <a name="saas-subscription-and-configuration"></a>Abonnement et configuration SaaS

Lorsque vous sélectionnez s’abonner, un message indique « votre abonnement SaaS est en cours ». Ce processus doit prendre quelques minutes, ne fermez pas la fenêtre tant que l’opération n’est pas terminée.

Une fois l’abonnement terminé, un message indique que votre abonnement SaaS est terminé, et vous devez configurer le compte pour qu’il commence à profiter de votre achat. Vous recevrez également un message électronique vous invitant à activer le nouvel abonnement. Si vous n’êtes pas celui qui configure le compte SaaS, transférez cet e-mail à la personne concernée.

Pour terminer le processus et commencer à utiliser le SaaS, vous devez commencer à configurer votre abonnement. En sélectionnant le bouton **configurer le compte maintenant** , vous êtes redirigé vers le site Web de l’éditeur.

Vous pouvez également vérifier l’état de votre abonnement en sélectionnant l’icône « cloche » dans le coin supérieur droit de l’en-tête.

Si vous ne terminez pas le processus de configuration dans les *30 jours*, cet abonnement Saas sera automatiquement *supprimé*. La facturation démarre une fois que votre compte est configuré sur le site Web de l’éditeur.

Les messages d’erreur que vous pouvez rencontrer pendant le processus sont les suivants :

- Le *nom de plan du plan sélectionné* ne peut pas être acheté sur un abonnement gratuit
  - Mettez à niveau votre compte https://aka.ms/UpgradeFreeSub . pour plus d’informations, consultez.

- L’achat a échoué parce que nous n’avons pas trouvé de carte de crédit valide ou de mode de paiement associé à votre abonnement Azure.
  - Utilisez un autre abonnement Azure, une carte de crédit ou un mode de paiement add\update pour cet abonnement, puis réessayez.

- Le *nom de plan du plan sélectionné pour le* *nom* de l’offre par l' *éditeur de* l’éditeur de l’offre n’est pas disponible pour l’achat selon les règles définies par votre administrateur informatique.
  - Contactez votre administrateur informatique.

- Le *nom du plan sélectionné* pour le *plan d’offre sélectionné par l'* *éditeur de* l’éditeur de l’offre n’est pas disponible pour l’achat en raison des paramètres de la place de marché privée effectués par l’administrateur informatique de votre locataire.
  - Contactez votre administrateur informatique

- L’achat a échoué, car le terme de facturation demandé est vide ou non valide.
  - Essayez d’acheter un autre terme de plan/facturation.

- L’achat a échoué parce que nous n’avons pas pu vérifier votre accord juridique de signature.
  - Reprise Si l’erreur persiste, essayez d’effectuer l’achat à l’aide d’un autre abonnement Azure ou contactez le support technique.

- L’achat de l’offre *offerID* par l’éditeur *PublisherId* a échoué. Cette offre n’est pas disponible actuellement pour l’achat.
  - Réessayez plus tard. Si, après une heure, vous continuez à recevoir ce message d’erreur, contactez le support technique.  

- L’achat du plan *planID* de l’offre *offerID* par l’éditeur *PublisherId* a échoué. Ce plan n’est pas disponible actuellement pour l’achat.
  - Réessayez plus tard. Si, après une heure, vous continuez à recevoir ce message d’erreur, contactez le support technique. 

- L' *adresse de messagerie* du client avec l’ID d’objet *ObjectID* n’a pas l’autorisation d’effectuer l’action *DeploymentValidationAction* sur l’étendue groupe de ressources *; DeploymentScope* ou l’étendue n’est pas valide.  
  - Vous obtiendrez ce message si vous n’avez pas les autorisations appropriées sur le groupe de ressources/abonnement Azure.  
    Si l’accès a été accordé récemment, actualisez vos informations d’identification.  
    Pour déployer des ressources dans un groupe de ressources, vous devez disposer au minimum d’un accès contributeur. Vérifiez l’état de votre accès sous **groupes de ressources** , puis **Access Control**. Cela indique qui est le « propriétaire », que vous pouvez demander à vous attribuer en tant que « contributeur ».

- L’abonnement utilisé pour cet achat n’autorise pas les achats sur la place de marché.  
  - Utilisez un autre abonnement ou demandez à votre administrateur de modifier la définition de cet abonnement, puis réessayez.

## <a name="next-steps"></a>Étapes suivantes

- Si vous avez déjà acheté une offre dans la place de marché, accédez à [facturation et](/marketplace/billing-invoicing) facturation.
- Vous pouvez également en savoir plus sur les options des [plans privés](/marketplace/private-offers) .
