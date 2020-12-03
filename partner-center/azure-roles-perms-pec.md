---
title: Rôles, autorisations pour le crédit gagné par le partenaire
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En savoir plus sur les rôles et les autorisations que les partenaires peuvent obtenir en tant que crédit gagné (PEC). Ils diffèrent des rôles à travailler dans l’espace partenaires.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8c36883dc7d12b7ea0ce8f2644dbac86595ab131
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534588"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Rôles et autorisations nécessaires pour obtenir un crédit gagné par le partenaire

Les rôles suivants correspondent aux niveaux d’autorisation qui déterminent si un partenaire est éligible pour les crédits acquis par le partenaire.

>[!Important]
>Ces rôles et autorisations ne sont pas les mêmes que les rôles et les autorisations dont un utilisateur a besoin pour travailler dans l’espace partenaires.

|**Rôle**   |**Description**   |**PEC éligible**   |
|-----------------|:------------------|:--------------|
|Propriétaire  |Vous gérez tout, y compris l’accès aux ressources.|Oui|
|Contributeur |Vous gérez tout sauf en accordant l’accès aux ressources.|Oui|
|Lecteur|Vous pouvez tout afficher, mais ne pas apporter de modifications|Non|
|ACRDelete|acr delete|Oui|
|ACRImageSigner|signataire d’image ACR|Oui|
|ACRPull|tirer (pull) acr|Oui|
|AcrPush|envoyer (push) acr|Oui|
|AcrQuarantineReader|lecteur de données de quarantaine ACR|Non|
|AcrQuarantineWriter| écriture de données de quarantaine ACR|Oui|
|Contributeur du service de gestion des API|Peut gérer le service et les API|Oui|
|Rôle d’opérateur du service Gestion des API|Peut gérer le service, mais pas les API|Oui|
|Rôle de lecteur du service Gestion des API|Accès en lecture seule au service et aux API|Non|
|Contributeur de composants Application Insights|Gère les composants de Application Insights|Oui|
|Débogueur de capture instantanée d’Application Insights|Autorise l’utilisateur à consulter et à télécharger les instantanés de débogage collectés à l’aide du débogueur de capture instantanée Application Insights. Ces autorisations ne sont pas incluses dans les rôles Propriétaire et Contributeur.|Oui|
Opérateur de travaux Automation | Permet de créer et de gérer des travaux avec des runbooks Automation. | Oui | 
Opérateur Automation | Les opérateurs d’Automation sont en mesure de démarrer, d’arrêter, de suspendre et de reprendre des travaux | Oui | 
Opérateur de runbook Automation | Propriétés de lecture du runbook : pour pouvoir créer des travaux depuis le runbook. | Oui | 
Contributeur Avere | Peut créer et gérer un cluster Avere vFXT. | Oui | 
Opérateur Avere | Utilisé par le cluster Avere vFXT pour gérer le cluster | Oui | 
Propriétaire de données Azure Event Hubs | Permet un accès complet aux ressources Azure Event Hubs. | Oui | 
Récepteur de données Azure Event Hubs | Permet d’obtenir un accès en réception aux ressources Azure Event Hubs. | Oui | 
Expéditeur de données Azure Event Hubs | Permet d’obtenir un accès en envoi aux ressources Azure Event Hubs. | Oui | 
Rôle d’administrateur de cluster Azure Kubernetes Service | Répertorie les actions relatives aux informations d’identification de l’administrateur du cluster. | Oui | 
Rôle d’utilisateur de cluster Azure Kubernetes Service | Répertorie les actions relatives aux informations d’identification de l’utilisateur du cluster. | Oui | 
Lecteur de données Azure Maps (préversion) | Octroie un accès pour lire les données liées au mappage à partir d’un compte Azure Maps. | Non | 
Propriétaire de données Azure Service Bus | Permet un accès total aux ressources Azure Service Bus. | Oui | 
Récepteur de données Azure Service Bus | Permet d’obtenir un accès en réception aux ressources Azure Service Bus. | Oui | 
Expéditeur de données Azure Service Bus | Permet d’obtenir un accès en envoi aux ressources Azure Service Bus. | Oui | 
Propriétaire de l’inscription Azure Stack | Permet de gérer les inscriptions Azure Stack. | Oui | 
Contributeur de sauvegarde | Permet de gérer le service de sauvegarde, mais pas de créer des coffres, ni d’accorder l’accès à d’autres personnes | Oui | 
Opérateur de sauvegarde | Permet de gérer des services de sauvegarde, à l’exception de la suppression de la sauvegarde, de la création de coffres et de l’octroi d’autorisations d’accès à d’autres personnes | Oui | 
Lecteur de sauvegarde | Peut afficher des services de sauvegarde, mais pas apporter des modifications | Non | 
Lecteur de facturation | Autorise l’accès en lecture aux données de facturation | Non | 
Contributeur BizTalk | Permet de gérer des services BizTalk, mais pas d’y accéder. | Oui | 
Accès au nœud du membre blockchain (préversion) | Permet d’accéder aux nœuds du membre blockchain | Oui | 
Contributeur blueprint | Peut gérer les définitions blueprint, mais ne peut pas les affecter. | Oui | 
Opérateur blueprint | Peut affecter des blueprints publiés existants, mais ne peut pas en créer de nouveaux. REMARQUE : Cela fonctionne uniquement si l’affectation est effectuée avec une identité managée affectée par l’utilisateur. | Oui | 
Contributeur de point de terminaison CDN | Peut gérer les points de terminaison CDN, mais ne peut pas accorder l’accès à d’autres utilisateurs. | Oui | 
Lecteur de point de terminaison CDN | Peut afficher des points de terminaison CDN, mais ne peut pas effectuer de modifications. | Non | 
Contributeur de profil CDN | Peut gérer des profils CDN et leurs points de terminaison, mais ne peut pas accorder l’accès à d’autres utilisateurs. | Oui | 
Lecteur de profil CDN | Peut afficher des profils CDN et leurs points de terminaison, mais ne peut pas y apporter des modifications. | Non | 
Contributeur de réseau classique | Permet de gérer des réseaux classiques, mais pas d’y accéder. | Oui | 
Contributeur de compte de stockage classique | Permet de gérer des comptes de stockage classiques, mais pas d’y accéder. | Oui | 
Rôle de service d’opérateur de clé de compte de stockage classique | Les opérateurs de clés de comptes de stockage classiques sont autorisés à lister et à régénérer des clés sur des comptes de stockage classiques | Oui | 
Contributeur de machine virtuelle classique | Permet de gérer des machines virtuelles classiques, mais pas d’y accéder, ni au réseau virtuel ou au compte de stockage auquel elles sont connectées. | Oui | 
Contributeur Cognitive Services | Vous permet de créer, lire, mettre à jour, supprimer et gérer les clés de Cognitive Services. | Oui | 
Lecteur de données Cognitive Services (préversion) | Permet de lire des données Cognitive Services. | Non | 
Utilisateur Cognitive Services | Vous permet de lire et de répertorier les clés de Cognitive Services. | Non | 
Rôle de lecteur de compte Cosmos DB | Lire les données de comptes Azure Cosmos DB. Consultez Contributeur de compte DocumentDB pour en savoir plus sur la gestion des comptes Azure Cosmos DB. | Non | 
Opérateur Cosmos DB | Permet de gérer des comptes Azure Cosmos DB, mais pas d’accéder aux données qu’ils contiennent. Empêche d’accéder aux clés de compte et aux chaînes de connexion. | Oui | 
CosmosBackupOperator | Peut envoyer une requête de restauration d’une base de données Cosmos DB ou d’un conteneur pour un compte | Oui | 
Contributeur Cost Management | Peut afficher les coûts et gérer la configuration des coûts (par exemple, budgets, exportations) | Oui | 
Lecteur Cost Management | Peut afficher les données et la configuration des coûts (par exemple, budgets, exportations) | Non | 
Contributeur Data Box | Permet de gérer toutes les opérations sous le service Data Box à l’exception de l’octroi d’accès à d’autres personnes. | Oui | 
Lecteur Data Box | Permet de gérer le service Data Box, mais ne permet pas de créer une commande, de modifier les détails d’une commande ou d’octroyer l’accès à d’autres personnes. | Non | 
Contributeurs de fabrique de données | Créer et gérer des fabriques de données, ainsi que les ressources enfants qu’elles contiennent. | Oui | 
Développeur Data Lake Analytics | Permet d’envoyer, de surveiller et de gérer vos propres travaux, mais pas de créer ni de supprimer des comptes Data Lake Analytics. | Oui | 
Videur de données | Peut vider les données d’analytique | Oui | 
Utilisateur de DevTest Labs | Permet de connecter, de démarrer, de redémarrer et d’arrêter vos machines virtuelles dans votre Azure DevTest Labs. | Oui | 
Contributeur de Zone DNS | Permet de gérer des zones DNS et des jeux d’enregistrements dans Azure DNS, mais pas de contrôler qui y a accès. | Oui | 
Contributeur de compte DocumentDB | Gérer des comptes Azure Cosmos DB. Azure Cosmos DB était auparavant appelé DocumentDB. | Oui | 
Contributeur EventGrid EventSubscription | Vous permet de gérer les opérations d’abonnement aux événements EventGrid. | Oui | 
Lecteur EventGrid EventSubscription | Vous permet de lire les abonnements aux événements EventGrid. | Non | 
Opérateur de cluster HDInsight | Permet de lire et de modifier des configurations de cluster HDInsight. | Oui | 
Contributeur HDInsight Domain Services | Peut lire, créer, modifier et supprimer les opérations Domain Services nécessaires pour le pack Sécurité Entreprise HDInsight | Oui | 
Contributeur de compte Intelligent Systems | Permet de gérer des comptes Intelligent Systems, mais pas d’y accéder. | Oui | 
Contributeur Key Vault | Permet de gérer des coffres de clés, mais pas d’y accéder. | Oui | 
Créateur Lab | Permet de créer, de gérer et de supprimer des labs gérés dans vos comptes Azure Lab. | Oui | 
Contributeur Log Analytics | Peut lire toutes les données de surveillance et modifier les paramètres de surveillance. La modification des paramètres de supervision inclut l’ajout de l’extension de machine virtuelle aux machines virtuelles, la lecture des clés de comptes de stockage permettant de configurer la collection de journaux d’activité du stockage Azure, la création et la configuration de comptes Automation, l’ajout de solutions et la configuration de diagnostics Azure sur toutes les ressources Azure. | Oui | 
Lecteur Log Analytics | Peut afficher et rechercher toutes les données de surveillance, ainsi qu’afficher les paramètres de surveillance, notamment la configuration des diagnostics Azure sur toutes les ressources Azure. | Non | 
Contributeur d’application logique | Permet de gérer des applications logiques, mais pas d’en modifier l’accès. | Oui | 
Opérateur d’application logique | Permet de lire, d’activer et de désactiver des applications logiques, mais pas de les modifier ou de les mettre à jour. | Oui | 
Rôle opérateur d’application managée | Permet de lire les ressources d’application managée et d’effectuer des actions sur ces ressources. | Oui | 
Lecteur Applications managées | Vous permet de lire les ressources dans une application managée et de demander un accès JIT. | Non | 
Contributeur d’identités gérées | Peut créer, lire, mettre à jour et supprimer une identité attribuée à l’utilisateur. | Oui | 
Opérateur d’identités gérées | Peut lire et assigner une identité attribuée à l’utilisateur. | Oui | 
Collaborateur du groupe d’administration | Rôle de collaborateur du groupe d’administration | Oui | 
Lecteur du groupe d’administration | Rôle de lecteur du groupe d’administration | Non | 
Contributeur d’analyse | Peut lire toutes les données de surveillance et modifier les paramètres de surveillance. Consultez aussi Bien démarrer avec les rôles, les autorisations et la sécurité dans Azure Monitor. | Oui | 
Publication des métriques de surveillance | Permet de publier les métriques relatives aux ressources Azure | Oui | 
Lecteur d’analyse | Peut lire toutes les données de supervision (métriques, journaux d’activité, etc.) Consultez aussi Bien démarrer avec les rôles, les autorisations et la sécurité dans Azure Monitor. | Non | 
Contributeur de réseau | Permet de gérer des réseaux, mais pas d’y accéder. | Oui | 
Contributeur de compte NewRelic APM | Vous permet de gérer des comptes et applications New Relic Application Performance Management, mais pas d’y accéder. | Oui | 
Lecteur et accès aux données | Permet d’afficher tous les éléments, mais pas de supprimer ou de créer un compte de stockage ou une ressource contenue. En outre, autorise l’accès en lecture/écriture à toutes les données contenues dans un compte de stockage via l’accès aux clés de compte de stockage. | Oui | 
Contributeur Cache Redis | Permet de gérer des caches Redis, mais pas d’y accéder. | Oui | 
Contributeur de stratégie de ressource (préversion) | (Préversion) Utilisateurs renvoyés de EA, avec des droits pour créer ou modifier une stratégie de ressource, créer un ticket de support et lire des ressources ou la hiérarchie. | Oui | 
Contributeur des collections de travaux du planificateur | Permet de gérer des collections de tâches du planificateur, mais pas d’y accéder. | Oui | 
Contributeur du service de recherche | Permet de gérer des services de recherche, mais pas d’y accéder. | Oui | 
Administrateur de la sécurité | Dans Security Center uniquement : peut afficher des stratégies de sécurité, afficher des états de sécurité, modifier des stratégies de sécurité, afficher des alertes et des recommandations, ignorer les alertes et les recommandations | Oui | 
Gestionnaire de sécurité (hérité) | Il s’agit d’un rôle hérité. Utilisez plutôt l’administrateur de sécurité. | Oui | 
Lecteur de sécurité | Dans Security Center uniquement : peut afficher des recommandations et des alertes, afficher des stratégies de sécurité, afficher des états de la sécurité, mais ne peut pas apporter des modifications | Non | 
Contributeur Site Recovery | Permet de gérer le service Site Recovery sauf la création de coffre et l’attribution de rôle | Oui | 
Opérateur Site Recovery | Permet de basculer et de restaurer mais pas d’effectuer d’autres opérations de gestion de Site Recovery | Oui | 
Lecteur Site Recovery | Permet d’afficher l’état de Site Recovery mais pas d’effectuer d’autres opérations de gestion | Non | 
Contributeur de compte Spatial Anchors | Permet de gérer des ancres spatiales dans votre compte, mais pas de les supprimer | Oui | 
Propriétaire de compte Spatial Anchors | Permet de gérer des ancres spatiales dans votre compte, y compris de les supprimer | Oui | 
Lecteur de compte Spatial Anchors | Permet de localiser et de lire les propriétés d’ancres spatiales dans votre compte | Non | 
Contributeur de base de données SQL | Permet de gérer des bases de données SQL, mais pas d’y accéder. Vous ne pouvez pas non plus gérer leurs stratégies de sécurité ni leurs serveurs SQL parents. | Oui | 
Contributeur d’Instance managée SQL | Permet de gérer des instances SQL Managed Instance et la configuration réseau requise, mais pas d’accorder l’accès à d’autres personnes. | Oui | 
Gestionnaire de sécurité SQL | Permet de gérer les stratégies de sécurité des serveurs et bases de données SQL, mais pas d’y accéder. | Oui | 
Contributeur SQL Server | Permet de gérer des serveurs et bases de données SQL, mais pas d’y accéder, ni de gérer leurs stratégies de sécurité. | Oui | 
Contributeur de compte de stockage | Permet la gestion des comptes de stockage. Fournit l’accès à la clé de compte, qui peut être utilisée pour accéder aux données par le biais de l’autorisation de clé partagée. | Oui | 
Rôle de service d’opérateur de clé de compte de stockage | Permet de répertorier et de régénérer les clés d’accès au compte de stockage. | Oui | 
Contributeur aux données Blob du stockage | Lire, écrire et supprimer des conteneurs et objets blob du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Oui | 
Propriétaire des données Blob du stockage | Fournit un accès total aux conteneurs d’objets blob et aux données du Stockage Azure, notamment l’attribution du contrôle d’accès POSIX. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Oui | 
Lecteur des données blob du stockage | Lire et répertorier des conteneurs et objets blob du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Non | 
Délégation du Stockage Blob | Obtenez une clé de délégation d’utilisateur qui peut être utilisée pour créer une signature d’accès partagé pour un conteneur ou un objet blob signé avec les informations d’identification Azure AD. Pour en savoir plus, consultez Créer une SAP de délégation d’utilisateur. | Oui | 
Collaborateur de partage SMB des données du fichier de stockage | Permet l'accès en lecture, en écriture et pour suppression dans des partages de fichiers Stockage Azure via SMB | Oui | 
Collaborateur à privilèges élevés de partage SMB des données du fichier de stockage | Permet l'accès en lecture, en écriture, pour suppression et pour modification dans des partages de fichiers Stockage Azure via SMB | Oui | 
Lecteur de partage SMB des données du fichier de stockage | Autorise l’accès en lecture au partage de fichiers Azure via SMB | Non | 
Contributeur aux données en file d’attente du stockage | Lire, écrire et supprimer des files d'attente et messages en file d'attente du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Oui | 
Processeur de messages de données en file d’attente du stockage | Récupérer et supprimer un message, ou en afficher un aperçu à partir d’une file d’attente Stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Oui | 
Expéditeur de messages de données en file d’attente du stockage | Ajoutez des messages à une file d’attente de stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Oui | 
Lecteur des données en file d’attente du stockage | Lire et répertorier des files d’attente et messages en file d’attente du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Non | 
Contributeur de demande de support | Permet de créer et de gérer des demandes de support | Oui | 
Contributeur Traffic Manager | Permet de gérer des profils Traffic Manager, mais pas de contrôler qui y a accès. | Oui | 
Administrateur de l'accès utilisateur | Vous permet de gérer l'accès utilisateur aux ressources Azure. | Oui | 
Connexion de l’administrateur aux machines virtuelles | Afficher les machines virtuelles dans le portail et se connecter en tant qu’administrateur | Oui | 
Contributeur de machine virtuelle | Permet de gérer des machines virtuelles, mais pas d’y accéder, ni au réseau virtuel ou au compte de stockage auquel elles sont connectées. | Oui | 
Connexion de l’utilisateur aux machines virtuelles | Affichez les machines virtuelles dans le portail et connectez-vous en tant qu’utilisateur normal. | Oui | 
Contributeur de plan web | Permet de gérer des plans web pour des sites web, mais pas d’y accéder. | Oui | 
Contributeur de site web | Vous permet de gérer des sites Web (pas des plans Web), mais pas d’y accéder | Oui |

## <a name="next-steps"></a>Étapes suivantes

- [Crédit Partenaires : vue d’ensemble de son fonctionnement dans la nouvelle expérience commerciale du fournisseur de solutions Cloud](partner-earned-credit.md)
