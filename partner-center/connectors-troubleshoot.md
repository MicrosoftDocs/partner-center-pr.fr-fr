---
title: Résoudre les problèmes des connecteurs de référencements de covente
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: FAQ sur la résolution des problèmes de co-vente des connecteurs.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: d34a13a6789f3bd712d2cec3a594b8e407f7449d
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422335"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Résoudre les problèmes des connecteurs de référencements de covente

**S’applique à :**

- Espace partenaires
- Dynamics 365 CRM
- CRM Salesforce

**Rôles appropriés**

- Administrateur des références
- Administrateur système ou personnalisateur de système sur le CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Questions et réponses sur les conditions préalables

1. Pouvez-vous utiliser une solution de connecteurs de références de co-vente d’essai pour votre environnement ?

Si vous êtes dans l’environnement test/intermédiaire, vous pouvez opter pour une solution d’évaluation. La version payante des connecteurs est disponible dans AppSource au 15 au mois. Avec la connexion payante, vous obtenez jusqu’à 10 000 appels d’API par jour. Les connecteurs sont des wrappers par-dessus les API de référence de l’espace partenaires. Chaque fois que les solutions de connecteur s’exécutent pour un événement de **création** ou de **mise à jour** sur les opportunités sur l’espace partenaires ou le côté CRM, un appel d’API est effectué.

2. Quel rôle avez-vous besoin pour créer des sections dans l’environnement CRM ?

Les utilisateurs qui sont des administrateurs système ou des personnalisateurs de systèmes peuvent appliquer des modifications pour tout le monde. Toutefois, tous les utilisateurs de l’application peuvent personnaliser le système et même partager certaines de leurs personnalisations avec d’autres utilisateurs. 

3. Les vendeurs partenaires ont-ils besoin de rôles spéciaux pour travailler sur l’espace partenaires ?
 
Le rôle « administrateur des références » doit être attribué aux vendeurs partenaires. Pour plus d’informations, reportez-vous à la [vue d’ensemble des autorisations] (Create-User-Accounts-and-Set-Permissions).

4. Quels sont les champs qui doivent être configurés en premier dans votre environnement CRM ? 

• Assurez-vous que votre devise est adaptée à votre emplacement et dans votre environnement CRM avec précision. • Votre équipe de vente doit être inscrite dans votre environnement CRM en tant qu’utilisateurs CRM.

5.  Quelles sont les conditions préalables requises pour la création d’un environnement Power automate ?

Pour utiliser l’environnement Power automate, vous avez besoin des éléments suivants :

- Une licence Power automate est requise.
- Un espace de stockage de 1 Go au minimum est requis.

6.  Avez-vous besoin d’un abonnement Dynamics 365 pour utiliser la solution de connecteurs Salesforce ?

La solution de connecteur Salesforce est de type « Dynamics Flow » qui prend en charge la synchronisation avec d’autres systèmes CRM. La solution ne nécessite pas que vous disposiez d’une instance Dynamics 365 ou d’un abonnement. Lors de l’installation de la solution Salesforce, une liste déroulante contenant les CD existants dans votre entreprise peut s’afficher. Vous devez sélectionner cet environnement. En outre, si vous obtenez l’erreur, nous n’avons pas pu trouver une organisation Dynamics 365 connectée à un utilisateur connecté», vous devrez créer un nouvel environnement pour le connecteur.

## <a name="questions-and-answers-about-configuration"></a>Questions et réponses sur la configuration

1. Que devez-vous faire si vous êtes confronté à l’erreur suivante lors de l’activation de flux dans Power Automated Platform ?

Erreur : la demande de Azure Resource Manager a échoué avec l’erreur : « {erreur » : {« code » : « WorkflowTriggerNotFound », « message » : « le déclencheur «e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 » du workflow « Manual » est introuvable.»}}». 

Suivez les étapes de dépannage suivantes :

- Supprimez la connexion CDS, puis recréez les connexions CDS.
- Activer et désactiver le workflow enfant 
- Supprimez la solution, puis réinstallez la solution. 

2.  Que devez-vous faire si vous êtes confronté à l’erreur suivante lors de l’ajout d’un connecteur de l’espace partenaires dans Power automatiser la plateforme ?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Message d’erreur nécessitant une connexion":::

Suivez cette étape de résolution des problèmes :

- Utilisez l’espace partenaires pour vous connecter à l’environnement Flow une seule fois (flow.microsoft.com).


3. Que devez-vous faire si vous recevez l’erreur suivante lors de l’activation de l’espace partenaires sur le Flow CRM dans Power Automated Platform ?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Message d’erreur nécessitant des mises à jour":::

Suivez les étapes de dépannage suivantes :

- Commencez par activer les deux flux enfants suivants avant d’activer l’espace partenaires dans le flux CRM.
      - Espace partenaires vers CRM-Helper (version préliminaire d’Insider)
      - Espace partenaires Microsoft : mises à jour de référence de la co-vente à CRM (version préliminaire d’Insider)

4. Que devez-vous faire lorsque vous n’êtes pas en mesure d’ajouter des connexions au Flow lorsque vous essayez de modifier le Flow ?

Vous ajoutez des connexions au Flow pendant que le workflow est en cours d’exécution et vous ajoutez à chaque Flow séparément.  Si la boîte de dialogue d’ajout de connexions ne s’ouvre pas automatiquement pendant la modification du flux, vous pouvez modifier chacune des étapes et sous-étapes des flux pour ajouter les connexions.

- Sélectionnez chaque Flow et modifiez-les individuellement.
- Développer toutes les étapes du Flow 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Étapes nécessitant des connexions":::

- Sélectionnez les étapes dans lesquelles une icône d’avertissement s’affiche et vous invite à associer des connexions et à ajouter des connexions. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Modifier le Flow étape par étape":::


5. Que devez-vous faire si les flux de la solution de références de covente des connexions ne sont pas activés (activation) ?

R. Dans Power automate, vous devrez modifier les flux dans l’ordre suivant et les mettre à jour pour qu’ils utilisent des connexions respectives :

- Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)
- Créer une référence de covente-Salesforce à l’espace partenaires (version préliminaire d’Insider)
- Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)
- Espace partenaires vers Salesforce (version préliminaire d’Insider)
- Salesforce pour Partner Center (version préliminaire d’Insider)
- Opportunité Salesforce pour Partner Center (version préliminaire d’Insider)
- Solutions Microsoft Salesforce pour Partner Center (version préliminaire d’Insider)

 B. Pour chaque Flow, sélectionnez l’option **exécuter uniquement les utilisateurs** . Sélectionnez **utiliser la connexion** au lieu de **fourni par l’utilisateur en exécution seule**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Pour activer un Flow":::


C. Activez les flux indiqués ci-dessous :

 - Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)

- Salesforce pour Partner Center (version préliminaire d’Insider)

    
D. Activez tous les flux restants.

E. Dans l’inscription au webhook de l’espace partenaires, sélectionnez **exécuter**. Fournissez l' **URL http** à partir de la première action dans **Partner Center vers Salesforce** Flow. Sélectionnez les quatre options sous **événements à inscrire** , puis sélectionnez **Oui** pour le remplacement.

## <a name="questions-and-answers-about-runmaintenance"></a>Questions et réponses sur l’exécution et la maintenance

1. Comment résoudre les problèmes en cas de défaillances lors de l’exécution d’automate Power ?

Pour vous assurer que vos flux d’automati s’exécutent comme prévu et pour résoudre les problèmes d’échec lors de l’exécution, reportez-vous à [corriger les échecs de flux](/power-automate/fix-flow-failures).

2. Que devez-vous faire si vous voyez des références qui ne sont pas correctement synchronisées dans l’espace partenaires ou l’environnement CRM ?
 
Pour déterminer l’état de synchronisation de la référence, sélectionnez **audit**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisation des références":::

Assurez-vous que les conditions suivantes sont remplies :

- L’ID de solution est fourni dans le cadre de l’opportunité.

- Un code de pays à deux lettres est requis.

- Lorsque l’aide de Microsoft est sélectionnée pour l’opportunité, les coordonnées du client sont requises.

3. Dans quelles conditions une référence ne sera pas synchronisée de manière bidirectionnelle

Vérifiez les points suivants :

- Les vendeurs partenaires doivent s’assurer qu’ils ont activé l’option **synchroniser avec l’espace partenaires** dans la section CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Vérifiez que vous avez activé la synchronisation":::

- Les vendeurs doivent fournir un chiffre d’affaires et une date de clôture lorsqu’ils qualifient un prospect.

- Si l’ID CRM est fourni lors de la création ou de la mise à jour de l’opportunité de covente et si un prospect/opportunité avec cet ID est introuvable dans CRM, la mise à jour ou la création sera ignorée pour cette opportunité.

- Assurez-vous que le champ devise de référence est configuré dans l’environnement Salesforce. 

4. Que devez-vous faire si le connecteur est déconnecté et que vous manquez une synchronisation de référence. 

Voici quelques-unes des options que vous pouvez essayer :

- Vérifiez si le nom d’utilisateur ou le mot de passe a expiré pour l’utilisateur de l’espace partenaires avec des rôles d’administrateur de référence.

- Vous pouvez accéder à l’opportunité non synchronisée, effectuer une mise à jour mineure et observer si la référence a été synchronisée.

- Si les flux ont été exécutés et ont échoué, sélectionnez le flux et soumettez à nouveau l’exécution qui a échoué.

5. Que devez-vous faire lorsque vous recevez des erreurs d’accès refusé ?

Assurez-vous que les rôles appropriés existent

- Rôle d’administrateur de référence pour le vendeur de l’espace partenaires 
 
- Rôle d’administrateur système ou de personnalisateur de système sur votre instance CRM

- Assurez-vous que l’utilisateur du compte de gestion de l’alimentation se connecte https://flow.microsoft.com au moins une fois au préalable

6. Si vous voyez que l' **indicatif du pays du compte client** est manquant lors de la création d’une opportunité de covente, que devez-vous faire ?

Vous devez ajouter le code du pays ISO à deux lettres au compte client dans CRM.

7. Que devez-vous faire si vous voyez l’erreur indiquant que l' **ID de solution est requis** lors de la création d’une opportunité de covente ?

Pour créer une référence de covente, vous avez besoin d’une solution Microsoft de co-vente prête. 

8. Que devez-vous faire lorsque vous voyez des opportunités de covente créées dans l’espace partenaires qui ne sont pas synchronisées avec CRM, même s’il n’y a pas d’erreurs de flow :

Effectuez les actions suivantes :

- Une fois que vous avez créé une nouvelle vente de covente dans l’espace partenaires, vérifiez si l’option espace partenaires pour Dynamics 365 Flow est invoquée (elle peut être appelée plusieurs fois).

- Si le flux est appelé, vérifiez tous les flux appelés et identifiez l’exécution du flux qui met à jour le CRM. Vous pouvez suivre les actions et vérifier si le service CRM a été mis à jour ou si un problème s’est produit.

- Cochez *nouveau contrat** dans l’espace partenaires pour voir s’il est rempli avec l’ID CRM.

- Assurez-vous que la transaction n’est pas fermée par erreur en tant que « gagné » ou « perdue » dans l’espace partenaires.

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les prospects](manage-leads.md)
 
- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)