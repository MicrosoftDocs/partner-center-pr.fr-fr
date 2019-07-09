---
title: Analytique de Microsoft Learn | Partenaires
ms.topic: article
ms.date: 07/05/2019
description: Pour plus d’informations sur la façon de comprendre votre analytique learning
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09d4ca14c1b407e9010ab26bccaf612f9caad732
ms.sourcegitcommit: bd83621eb29fafbda341ad41814a9ae5c1e78b00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/08/2019
ms.locfileid: "67622527"
---
# <a name="microsoft-learn-analytics-report"></a>Rapport d’analytique Microsoft Learn

Le rapport Microsoft Learn vous fournit des informations sur les apprenants dans votre entreprise, y compris les modules qu’ils ont effectuées et ils se trouvent sur les parcours d’apprentissage. Le rapport affiche l’état de chaque apprenant individuel. L’administrateur général et l’administrateur MPN pour votre entreprise peuvent afficher les données.

## <a name="how-to-read-the-report"></a>Guide pratique pour lire le rapport

### <a name="summary-charts"></a>Graphiques de résumé

**Formé le nombre de personnes**: Nombre de tous les apprenants distincts qui ont effectué au moins un module au cours de la plage de dates sélectionnée 

**Mini graphique de tendance aux individus**: Mois au nombre cumulé de mois des apprenants actives 

**Nombre de saisies semi-automatiques modules**: Nombre de Module saisie semi-automatique par les apprenants de la société partenaire au cours de la plage de dates sélectionnée.
Par exemple, si « Module 1 » est effectué par des 15 personnes et le « Module 2" a été effectuée par les mêmes 15 personnes, le nombre de saisies semi-automatiques de module est 30. La date de fin de module doit se situent dans la plage de dates sélectionnée.

**Mini graphique de tendance des saisies semi-automatiques module**: Mois au nombre cumulé de mois de la saisie semi-automatique de module 

**Nombre de saisies semi-automatiques de chemin d’accès d’apprentissage**: Nombre de Learning chemin d’accès saisie semi-automatique par les apprenants de la société partenaire au cours de la plage de dates sélectionnée.
Par exemple, si le parcours d’apprentissage « Chemin d’accès 1 » est effectuée par 20 personnes et le parcours d’apprentissage « chemin d’accès 2" a été effectuée par les mêmes 20 personnes, le nombre de saisie semi-automatique du parcours d’apprentissage est 40. La date de fin du chemin d’accès Learning doit appartenir au sein de la plage de dates sélectionnée.

**Mini graphique de tendance des saisies semi-automatiques de chemin d’accès d’apprentissage**: Mois au nombre cumulé de mois de l’apprentissage saisies semi-automatiques de chemin d’accès 

### <a name="trained-individuals-monthly-trend"></a>Tendance des individus formé mensuels

**Axe des abscisses** est mois pour le filtre de temps sélectionné. 

**L’axe des y** est le nombre d’apprenants actives qui se sont inscrits (la première saisie semi-automatique d’un module) au cours du mois. Cela n’est pas cumulatif.

### <a name="module-completions-monthly-trend"></a>Tendance mensuelle des saisies semi-automatiques de module

**Axe des abscisses** est mois pour le filtre de temps sélectionné. 

**L’axe des y** est le nombre des saisies semi-automatiques module au cours du mois. Cela n’est pas cumulatif.

### <a name="learning-path-completions-monthly-trend"></a>Tendance mensuelle des saisies semi-automatiques chemin Learning

**Axe des abscisses** est mois pour le filtre de temps sélectionné. 

**L’axe des y** est le nombre de saisies semi-automatiques de module dans ce mois. Cela n’est pas cumulatif.

### <a name="learning-path-completion-tabs"></a>Onglets de saisie semi-automatique de chemin d’accès d’apprentissage 

- Onglet de module

**Graphique en anneau de saisies semi-automatiques module**: répartition de la saisie semi-automatique de module (nombre affiché dans la section résumée) par les noms de module.

Nombre affiché dans le centre du graphique est les total modules terminées

**Les saisies semi-automatiques par rôle**: répartition des saisies semi-automatiques module par le rôle du module. Si un module est associé à plusieurs rôles, chacun des rôles est ajouté au nombre de saisies semi-automatiques de module.

Nombre affiché dans le centre du graphique en anneau est le nombre de rôles distincts pour les saisies semi-automatiques de module. 

**Les saisies semi-automatiques par produit**: répartition de la saisie semi-automatique de module par le produit, le module est mappé à. Si un module est associé à plusieurs produits, chaque produit est ajoutée au nombre de saisies semi-automatiques de module.    

Nombre affiché au milieu du graphique en anneau est le nombre de produits distincts pour les saisies semi-automatiques de module.  

- Onglet chemin d’accès de formation    

**Graphique en anneau de saisies semi-automatiques chemins d’apprentissage**: répartition des saisies semi-automatiques de chemins d’accès d’apprentissage (nombre affiché dans la section résumée) par nom.

**Les saisies semi-automatiques par rôle**: répartition de l’apprentissage saisies semi-automatiques de chemins d’accès par le rôle. Si un module est associé à plusieurs rôles, chacun des rôles est ajouté au nombre de saisies semi-automatiques de module.

**Les saisies semi-automatiques par produit**: répartition de l’apprentissage saisies semi-automatiques de chemins d’accès par le produit à laquelle le parcours d’apprentissage est mappée. Si un module est associé à plusieurs produits, chaque produit est ajoutée au nombre de saisies semi-automatiques de module.

### <a name="completions-by-learning-individuals"></a>Les saisies semi-automatiques en apprenant les individus

Microsoft Learn identifie les apprenants avec un ID d’objet utilisateur. Sous le **onglet Modules**, tous les apprenants sont triés par les modules terminées. Ils sont affichés avec leur nom d’utilisateur Microsoft Learn, ID d’objet et le nombre de modules. Vous pouvez rechercher à l’aide du nom d’utilisateur.

Pour obtenir des détails d’un apprenant à l’aide de l’ID d’objet utilisateur : 

1. Connectez-vous à [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Vous devez être administrateur général du locataire Azure AD de votre société.)

2. Copiez l’ID d’objet utilisateur pour le [mis en surbrillance de zone](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) dans l’Explorateur graphique. 

