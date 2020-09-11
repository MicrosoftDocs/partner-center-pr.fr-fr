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
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011739"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Rôles et autorisations admissibles pour obtenir un crédit gagné par le partenaire

Les rôles suivants correspondent aux niveaux d’autorisation qui déterminent si un partenaire est éligible pour les crédits acquis par le partenaire.

>[!Important]
>Ces rôles et autorisations ne sont pas les mêmes que les rôles et les autorisations dont un utilisateur a besoin pour travailler dans l’espace partenaires.

|**Rôle**   |**Description**   |**PEC éligible**   |
|-----------------|:------------------|:--------------|
|Propriétaire  |Vous gérez tout, y compris l’accès aux ressources.|Yes|
|Contributeur |Vous gérez tout sauf en accordant l’accès aux ressources.|Yes|
|Lecteur|Vous pouvez tout afficher, mais ne pas apporter de modifications|No|
|ACRDelete|acr delete|Yes|
|ACRImageSigner|signataire d’image ACR|Yes|
|ACRPull|tirer (pull) acr|Yes|
|AcrPush|envoyer (push) acr|Yes|
|AcrQuarantineReader|lecteur de données de quarantaine ACR|No|
|AcrQuarantineWriter| écriture de données de quarantaine ACR|Yes|
|Contributeur du service de gestion des API|Peut gérer le service et les API|Yes|
|Rôle d’opérateur du service Gestion des API|Peut gérer le service, mais pas les API|Yes|
|Rôle de lecteur du service Gestion des API|Accès en lecture seule au service et aux API|No|
|Contributeur de composants Application Insights|Gère les composants de Application Insights|Yes|
|Débogueur de capture instantanée d’Application Insights|Autorise l’utilisateur à consulter et à télécharger les instantanés de débogage collectés à l’aide du débogueur de capture instantanée Application Insights. Ces autorisations ne sont pas incluses dans les rôles Propriétaire et Contributeur.|Yes|
Opérateur de travaux Automation | Permet de créer et de gérer des travaux avec des runbooks Automation. | Yes | 
Opérateur Automation | Les opérateurs d’Automation sont en mesure de démarrer, d’arrêter, de suspendre et de reprendre des travaux | Yes | 
Opérateur de runbook Automation | Propriétés de lecture du runbook : pour pouvoir créer des travaux depuis le runbook. | Yes | 
Contributeur Avere | Peut créer et gérer un cluster Avere vFXT. | Yes | 
Opérateur Avere | Utilisé par le cluster Avere vFXT pour gérer le cluster | Yes | 
Propriétaire de données Azure Event Hubs | Permet un accès complet aux ressources Azure Event Hubs. | Yes | 
Récepteur de données Azure Event Hubs | Permet d’obtenir un accès en réception aux ressources Azure Event Hubs. | Yes | 
Expéditeur de données Azure Event Hubs | Permet d’obtenir un accès en envoi aux ressources Azure Event Hubs. | Yes | 
Rôle d’administrateur de cluster Azure Kubernetes Service | Répertorie les actions relatives aux informations d’identification de l’administrateur du cluster. | Yes | 
Rôle d’utilisateur de cluster Azure Kubernetes Service | Répertorie les actions relatives aux informations d’identification de l’utilisateur du cluster. | Yes | 
Lecteur de données Azure Maps (préversion) | Octroie un accès pour lire les données liées au mappage à partir d’un compte Azure Maps. | No | 
Propriétaire de données Azure Service Bus | Permet un accès total aux ressources Azure Service Bus. | Yes | 
Récepteur de données Azure Service Bus | Permet d’obtenir un accès en réception aux ressources Azure Service Bus. | Yes | 
Expéditeur de données Azure Service Bus | Permet d’obtenir un accès en envoi aux ressources Azure Service Bus. | Yes | 
Propriétaire de l’inscription Azure Stack | Permet de gérer les inscriptions Azure Stack. | Yes | 
Contributeur de sauvegarde | Permet de gérer le service de sauvegarde, mais pas de créer des coffres, ni d’accorder l’accès à d’autres personnes | Yes | 
Opérateur de sauvegarde | Permet de gérer des services de sauvegarde, à l’exception de la suppression de la sauvegarde, de la création de coffres et de l’octroi d’autorisations d’accès à d’autres personnes | Yes | 
Lecteur de sauvegarde | Peut afficher des services de sauvegarde, mais pas apporter des modifications | No | 
Lecteur de facturation | Autorise l’accès en lecture aux données de facturation | No | 
Contributeur BizTalk | Permet de gérer des services BizTalk, mais pas d’y accéder. | Yes | 
Accès au nœud du membre blockchain (préversion) | Permet d’accéder aux nœuds du membre blockchain | Yes | 
Contributeur blueprint | Peut gérer les définitions blueprint, mais ne peut pas les affecter. | Yes | 
Opérateur blueprint | Peut affecter des blueprints publiés existants, mais ne peut pas en créer de nouveaux. REMARQUE : Cela fonctionne uniquement si l’affectation est effectuée avec une identité managée affectée par l’utilisateur. | Yes | 
Contributeur de point de terminaison CDN | Peut gérer les points de terminaison CDN, mais ne peut pas accorder l’accès à d’autres utilisateurs. | Yes | 
Lecteur de point de terminaison CDN | Peut afficher des points de terminaison CDN, mais ne peut pas effectuer de modifications. | No | 
Contributeur de profil CDN | Peut gérer des profils CDN et leurs points de terminaison, mais ne peut pas accorder l’accès à d’autres utilisateurs. | Yes | 
Lecteur de profil CDN | Peut afficher des profils CDN et leurs points de terminaison, mais ne peut pas y apporter des modifications. | No | 
Contributeur de réseau classique | Permet de gérer des réseaux classiques, mais pas d’y accéder. | Yes | 
Contributeur de compte de stockage classique | Permet de gérer des comptes de stockage classiques, mais pas d’y accéder. | Yes | 
Rôle de service d’opérateur de clé de compte de stockage classique | Les opérateurs de clés de comptes de stockage classiques sont autorisés à lister et à régénérer des clés sur des comptes de stockage classiques | Yes | 
Contributeur de machine virtuelle classique | Permet de gérer des machines virtuelles classiques, mais pas d’y accéder, ni au réseau virtuel ou au compte de stockage auquel elles sont connectées. | Yes | 
Contributeur Cognitive Services | Vous permet de créer, lire, mettre à jour, supprimer et gérer les clés de Cognitive Services. | Yes | 
Lecteur de données Cognitive Services (préversion) | Permet de lire des données Cognitive Services. | No | 
Utilisateur Cognitive Services | Vous permet de lire et de répertorier les clés de Cognitive Services. | No | 
Rôle de lecteur de compte Cosmos DB | Lire les données de comptes Azure Cosmos DB. Consultez Contributeur de compte DocumentDB pour en savoir plus sur la gestion des comptes Azure Cosmos DB. | No | 
Opérateur Cosmos DB | Permet de gérer des comptes Azure Cosmos DB, mais pas d’accéder aux données qu’ils contiennent. Empêche d’accéder aux clés de compte et aux chaînes de connexion. | Yes | 
CosmosBackupOperator | Peut envoyer une requête de restauration d’une base de données Cosmos DB ou d’un conteneur pour un compte | Yes | 
Contributeur Cost Management | Peut afficher les coûts et gérer la configuration des coûts (par exemple, budgets, exportations) | Yes | 
Lecteur Cost Management | Peut afficher les données et la configuration des coûts (par exemple, budgets, exportations) | No | 
Contributeur Data Box | Permet de gérer toutes les opérations sous le service Data Box à l’exception de l’octroi d’accès à d’autres personnes. | Yes | 
Lecteur Data Box | Permet de gérer le service Data Box, mais ne permet pas de créer une commande, de modifier les détails d’une commande ou d’octroyer l’accès à d’autres personnes. | No | 
Contributeurs de fabrique de données | Créer et gérer des fabriques de données, ainsi que les ressources enfants qu’elles contiennent. | Yes | 
Développeur Data Lake Analytics | Permet d’envoyer, de surveiller et de gérer vos propres travaux, mais pas de créer ni de supprimer des comptes Data Lake Analytics. | Yes | 
Videur de données | Peut vider les données d’analytique | Yes | 
Utilisateur de DevTest Labs | Permet de connecter, de démarrer, de redémarrer et d’arrêter vos machines virtuelles dans votre Azure DevTest Labs. | Yes | 
Contributeur de Zone DNS | Permet de gérer des zones DNS et des jeux d’enregistrements dans Azure DNS, mais pas de contrôler qui y a accès. | Yes | 
Contributeur de compte DocumentDB | Gérer des comptes Azure Cosmos DB. Azure Cosmos DB était auparavant appelé DocumentDB. | Yes | 
Contributeur EventGrid EventSubscription | Vous permet de gérer les opérations d’abonnement aux événements EventGrid. | Yes | 
Lecteur EventGrid EventSubscription | Vous permet de lire les abonnements aux événements EventGrid. | No | 
Opérateur de cluster HDInsight | Permet de lire et de modifier des configurations de cluster HDInsight. | Yes | 
Contributeur HDInsight Domain Services | Peut lire, créer, modifier et supprimer les opérations Domain Services nécessaires pour le pack Sécurité Entreprise HDInsight | Yes | 
Contributeur de compte Intelligent Systems | Permet de gérer des comptes Intelligent Systems, mais pas d’y accéder. | Yes | 
Contributeur Key Vault | Permet de gérer des coffres de clés, mais pas d’y accéder. | Yes | 
Créateur Lab | Permet de créer, de gérer et de supprimer des labs gérés dans vos comptes Azure Lab. | Yes | 
Contributeur Log Analytics | Peut lire toutes les données de surveillance et modifier les paramètres de surveillance. La modification des paramètres de supervision inclut l’ajout de l’extension de machine virtuelle aux machines virtuelles, la lecture des clés de comptes de stockage permettant de configurer la collection de journaux d’activité du stockage Azure, la création et la configuration de comptes Automation, l’ajout de solutions et la configuration de diagnostics Azure sur toutes les ressources Azure. | Yes | 
Lecteur Log Analytics | Peut afficher et rechercher toutes les données de surveillance, ainsi qu’afficher les paramètres de surveillance, notamment la configuration des diagnostics Azure sur toutes les ressources Azure. | No | 
Contributeur d’application logique | Permet de gérer des applications logiques, mais pas d’en modifier l’accès. | Yes | 
Opérateur d’application logique | Permet de lire, d’activer et de désactiver des applications logiques, mais pas de les modifier ou de les mettre à jour. | Yes | 
Rôle opérateur d’application managée | Permet de lire les ressources d’application managée et d’effectuer des actions sur ces ressources. | Yes | 
Lecteur Applications managées | Vous permet de lire les ressources dans une application managée et de demander un accès JIT. | No | 
Contributeur d’identités gérées | Peut créer, lire, mettre à jour et supprimer une identité attribuée à l’utilisateur. | Yes | 
Opérateur d’identités gérées | Peut lire et assigner une identité attribuée à l’utilisateur. | Yes | 
Collaborateur du groupe d’administration | Rôle de collaborateur du groupe d’administration | Yes | 
Lecteur du groupe d’administration | Rôle de lecteur du groupe d’administration | No | 
Contributeur d’analyse | Peut lire toutes les données de surveillance et modifier les paramètres de surveillance. Consultez aussi Bien démarrer avec les rôles, les autorisations et la sécurité dans Azure Monitor. | Yes | 
Publication des métriques de surveillance | Permet de publier les métriques relatives aux ressources Azure | Yes | 
Lecteur d’analyse | Peut lire toutes les données de supervision (métriques, journaux d’activité, etc.) Consultez aussi Bien démarrer avec les rôles, les autorisations et la sécurité dans Azure Monitor. | No | 
Contributeur de réseau | Permet de gérer des réseaux, mais pas d’y accéder. | Yes | 
Contributeur de compte NewRelic APM | Vous permet de gérer des comptes et applications New Relic Application Performance Management, mais pas d’y accéder. | Yes | 
Lecteur et accès aux données | Permet d’afficher tous les éléments, mais pas de supprimer ou de créer un compte de stockage ou une ressource contenue. En outre, autorise l’accès en lecture/écriture à toutes les données contenues dans un compte de stockage via l’accès aux clés de compte de stockage. | Yes | 
Contributeur Cache Redis | Permet de gérer des caches Redis, mais pas d’y accéder. | Yes | 
Contributeur de stratégie de ressource (préversion) | (Préversion) Utilisateurs renvoyés de EA, avec des droits pour créer ou modifier une stratégie de ressource, créer un ticket de support et lire des ressources ou la hiérarchie. | Yes | 
Contributeur des collections de travaux du planificateur | Permet de gérer des collections de tâches du planificateur, mais pas d’y accéder. | Yes | 
Contributeur du service de recherche | Permet de gérer des services de recherche, mais pas d’y accéder. | Yes | 
Administrateur de la sécurité | Dans Security Center uniquement : peut afficher des stratégies de sécurité, afficher des états de sécurité, modifier des stratégies de sécurité, afficher des alertes et des recommandations, ignorer les alertes et les recommandations | Yes | 
Gestionnaire de sécurité (hérité) | Il s’agit d’un rôle hérité. Utilisez plutôt l’administrateur de sécurité. | Yes | 
Lecteur de sécurité | Dans Security Center uniquement : peut afficher des recommandations et des alertes, afficher des stratégies de sécurité, afficher des états de la sécurité, mais ne peut pas apporter des modifications | No | 
Contributeur Site Recovery | Permet de gérer le service Site Recovery sauf la création de coffre et l’attribution de rôle | Yes | 
Opérateur Site Recovery | Permet de basculer et de restaurer mais pas d’effectuer d’autres opérations de gestion de Site Recovery | Yes | 
Lecteur Site Recovery | Permet d’afficher l’état de Site Recovery mais pas d’effectuer d’autres opérations de gestion | No | 
Contributeur de compte Spatial Anchors | Permet de gérer des ancres spatiales dans votre compte, mais pas de les supprimer | Yes | 
Propriétaire de compte Spatial Anchors | Permet de gérer des ancres spatiales dans votre compte, y compris de les supprimer | Yes | 
Lecteur de compte Spatial Anchors | Permet de localiser et de lire les propriétés d’ancres spatiales dans votre compte | No | 
Contributeur de base de données SQL | Permet de gérer des bases de données SQL, mais pas d’y accéder. Vous ne pouvez pas non plus gérer leurs stratégies de sécurité ni leurs serveurs SQL parents. | Yes | 
Contributeur d’Instance managée SQL | Permet de gérer des instances SQL Managed Instance et la configuration réseau requise, mais pas d’accorder l’accès à d’autres personnes. | Yes | 
Gestionnaire de sécurité SQL | Permet de gérer les stratégies de sécurité des serveurs et bases de données SQL, mais pas d’y accéder. | Yes | 
Contributeur SQL Server | Permet de gérer des serveurs et bases de données SQL, mais pas d’y accéder, ni de gérer leurs stratégies de sécurité. | Yes | 
Contributeur de compte de stockage | Permet la gestion des comptes de stockage. Fournit l’accès à la clé de compte, qui peut être utilisée pour accéder aux données par le biais de l’autorisation de clé partagée. | Yes | 
Rôle de service d’opérateur de clé de compte de stockage | Permet de répertorier et de régénérer les clés d’accès au compte de stockage. | Yes | 
Contributeur aux données Blob du stockage | Lire, écrire et supprimer des conteneurs et objets blob du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Yes | 
Propriétaire des données Blob du stockage | Fournit un accès total aux conteneurs d’objets blob et aux données du Stockage Azure, notamment l’attribution du contrôle d’accès POSIX. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Yes | 
Lecteur des données blob du stockage | Lire et répertorier des conteneurs et objets blob du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | No | 
Délégation du Stockage Blob | Obtenez une clé de délégation d’utilisateur qui peut être utilisée pour créer une signature d’accès partagé pour un conteneur ou un objet blob signé avec les informations d’identification Azure AD. Pour en savoir plus, consultez Créer une SAP de délégation d’utilisateur. | Yes | 
Contributeur de partage SMB de données de fichier de stockage | Permet l'accès en lecture, en écriture et pour suppression dans des partages de fichiers Stockage Azure via SMB | Yes | 
Contributeur élevé de partage SMB de données de fichier de stockage | Permet l'accès en lecture, en écriture, pour suppression et pour modification dans des partages de fichiers Stockage Azure via SMB | Yes | 
Lecteur de partage SMB de données de fichier de stockage | Autorise l’accès en lecture au partage de fichiers Azure via SMB | No | 
Contributeur aux données en file d’attente du stockage | Lire, écrire et supprimer des files d'attente et messages en file d'attente du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Yes | 
Processeur de messages de données en file d’attente du stockage | Récupérer et supprimer un message, ou en afficher un aperçu à partir d’une file d’attente Stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Yes | 
Expéditeur de messages de données en file d’attente du stockage | Ajoutez des messages à une file d’attente de stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | Yes | 
Lecteur des données en file d’attente du stockage | Lire et répertorier des files d’attente et messages en file d’attente du stockage Azure. Pour savoir quelles actions sont requises pour une opération de données spécifique, consultez Autorisations pour appeler les opérations de données d’objet blob et de file d’attente. | No | 
Contributeur de demande de support | Permet de créer et de gérer des demandes de support | Yes | 
Contributeur Traffic Manager | Permet de gérer des profils Traffic Manager, mais pas de contrôler qui y a accès. | Yes | 
Administrateur de l'accès utilisateur | Vous permet de gérer l'accès utilisateur aux ressources Azure. | Yes | 
Connexion de l’administrateur aux machines virtuelles | Afficher les machines virtuelles dans le portail et se connecter en tant qu’administrateur | Yes | 
Contributeur de machine virtuelle | Permet de gérer des machines virtuelles, mais pas d’y accéder, ni au réseau virtuel ou au compte de stockage auquel elles sont connectées. | Yes | 
Connexion de l’utilisateur aux machines virtuelles | Affichez les machines virtuelles dans le portail et connectez-vous en tant qu’utilisateur normal. | Yes | 
Contributeur de plan web | Permet de gérer des plans web pour des sites web, mais pas d’y accéder. | Yes | 
Contributeur de site web | Vous permet de gérer des sites Web (pas des plans Web), mais pas d’y accéder | Oui |
