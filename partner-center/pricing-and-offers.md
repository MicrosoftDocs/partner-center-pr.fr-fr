---
title: Tarification et offres | Espace partenaires
ms.topic: article
ms.date: 09/26/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La liste des offres inclut les différentes familles de produits qui peuvent être achetées via l’espace partenaires et leurs informations de tarification.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e037f9e417da65ddd3d34fcdc7198807164906f9
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73654137"
---
# <a name="pricing-and-offers"></a>Tarification et offres

**S’applique à**

-  Espace partenaires

Pour afficher les dernières listes de prix et offres du programme Fournisseur de solutions Cloud, accédez à **Vendre > Tarification et offres**. Vous trouverez des listes de prix distinctes pour les services basés sur les licences, notamment Office 365, Microsoft Dynamics CRM, et Enterprise Mobility Suite et pour les services basés sur l’utilisation, comprenant Microsoft Azure. 

La liste des offres inclut les différentes familles de produits qui peuvent être achetées par le biais de l’espace partenaires. Il s’agit actuellement d’Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM et Microsoft Azure. D’autres produits seront ajoutés à cette liste.

Pour chaque famille de produits, il existe plusieurs références et offres groupées disponibles à la vente, selon votre activité. Vous pouvez toujours accéder aux détails les plus récents pour chaque produit à partir du tableau des offres des revendeurs cloud de la page Tarification et offres.

## <a name="pricelist-preview-and-change-frequency"></a>Aperçu de liste de prix et fréquence de modification 

Les services basés sur les licences incluent un aperçu de la liste de prix, fourni 30 jours avant toute modification. Pour afficher l’aperçu de la liste de prix, accédez à **Vendre > Tarification et offres**. Aucun aperçu de prix n’est fourni pour les services basés sur l’utilisation, car ces services sont dynamiques. Le tableau suivant explique comment interpréter le tableau de liste de prix.

|**Élément**        |**Définition**      |
|:-----------   |:-----------   |
|ADD   |Nouvel élément dans la liste de prix|
|CHG   |Modifications du tarif du mois au mois. D’autres modifications non liées au tarif de la liste peuvent se produire, les partenaires doivent comparer les autres propriétés du mois au mois pour déterminer d’autres modifications.|
|DEL   |Élément supprimé de la liste de prix|
|UNC   |Tarif non modifié à partir du pricelist du mois précédent  |
|Valide à partir du   |Première date à laquelle une offre peut être commandée    |
|Valide jusqu’au   |Date limite jusqu’à laquelle une offre peut être commandée   |
|Nom d’affichage de l’offre   |Nom de l’offre utilisé pour les clients   |
|ID de l’offre   |Identificateur interne de l’offre   |
|Type de contrat de licence   |Le type de contrat peut être professionnel, gouvernemental ou académique et il détermine à quels types de clients l’offre peut être vendue.|
|Unité d’achat   |Il s’agit de la durée de l’offre achetée. Elle est généralement d’un mois.   |
|Type de licence secondaire   |Il s’agit soit d’une offre non spécifique, d’une extension ou d’une version d’évaluation. Extension indique que le client doit acheter des logiciels requis avant d’acheter l’extension.|
|Type de client final   |Se rapporte au type de contrat de licence : licence d’entreprise - entreprise du revendeur cloud, licence gouvernementale - gouvernement du revendeur cloud ou licence pour établissements scolaires - corps enseignant du revendeur cloud ou étudiant du revendeur cloud   |
|Liste de prix   |Prix payé par le partenaire   |
|Prix moyen estimé   |Prix de vente au détail estimé ou recommandé pour le client   |

## <a name="price-changes"></a>Changements de prix

Les changements de prix sont des événements fréquents. Les partenaires peuvent anticiper les changements de prix pour les offres basées sur les licences en regardant la liste de prix dans la page tarification et offres du tableau de bord de l’espace partenaires. La tarification basée sur l’utilisation Azure n’a pas de préversion. Les partenaires peuvent suivre les changements de prix de la consommation Azure à l’aide de l’API RateCard qui retourne la tarification du compteur de ce jour.

|**Type de produit**   |**Exemples de produits**  |**Aperçu disponible** |**Modifier les détails**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basé sur une licence|Office, Dynamics, Intune, Windows entreprise|30 jours|Répertorier les modifications de prix marquées CHNG dans les listes de prix en version préliminaire|
|Basé sur l’utilisation|Ressources Azure|Non disponible|Journal des modifications disponible dans l’onglet **historique des modifications** de la liste de prix du mois précédent|
|Logiciels||Non disponible|Comparer les listes de prix manuellement du mois au mois|
|Effectuées|Machines virtuelles, prépayé|Non disponible|Comparer les listes de prix manuellement du mois au mois|

Les prix basés sur l’utilisation peuvent changer au cours d’un mois. Pour obtenir la tarification quotidienne « actuelle » pour ces ressources Azure, les partenaires doivent appeler l’API RateCard. 

>[!Note] 
>Les changements de prix des abonnements s’appliquent uniquement lors d’un renouvellement. Les frais mensuels d’un partenaire sont déterminés au prix de l’achat ou au prix au moment de la création d’un abonnement. Si un prix augmente ou diminue après l’acquisition du terme annuel, le partenaire ne facture pas le prix modifié jusqu’au renouvellement, généralement à la période de 12 mois.

## <a name="pricing-and-special-segments"></a>Tarification et segments spéciaux

Le fournisseur CSP offre des services à des segments de marché spéciaux, par exemple, l’éducation, le non-bénéfice et le Cloud de la communauté gouvernementale. Tous les services ne sont pas disponibles dans tous les canaux. Aucun segment n’a pour valeur par défaut ce que nous appelons le segment « commercial ». Toutes les tarifs basés sur les licences sont disponibles dans la liste des prix basés sur des licences sur la page tarification et offres. La tarification d’Azure gov est disponible dans la liste de prix basée sur l’utilisation lors de la connexion au locataire CSP activé pour Azure gov.

|**Partie**   |**qui doit être qualifié**   |**Le partenaire qualifie le client**|**Types de produits activés**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Éducation|Partenaire et client|Oui|Basée sur une licence uniquement|
|À but non lucratif|Client|Non, le client répond à l’extérieur de l’espace partenaires|Basée sur une licence uniquement|
|Government Community Cloud (GCC)|Partenaire et client|Une fois que GCC est activé, le partenaire peut créer des clients GCC| Basée sur une licence uniquement|
|Azure gov|Partenaire|Une fois qualifié, le partenaire travaille dans un locataire CSP spécifique à Azure gov|Ressources Azure|

Les marges du partenaire, la différence entre le tarif et les prix estimés au détail, peuvent varier d’un segment à l’autre. En règle générale, l’enseignement et le non-bénéfice ont tendance à avoir des marges inférieures ou égales pour les partenaires CSP. Reportez-vous à la liste des prix basés sur une licence pour obtenir les valeurs exactes.  
## <a name="pricing-between-azure-and-non-azure"></a>Tarification entre Azure et non-Azure

La tarification diffère selon les différents types d’offres. La tarification basée sur les licences est généralement le montant par poste (licence) pour un mois donné. La tarification basée sur l’utilisation est déterminée par l’utilisation d’une ressource donnée, avec un ID de compteur associé. Les partenaires ne sont pas facturés pour l’acquisition de l’abonnement Azure, mais sont facturés pour les ressources consommées par différents déploiements dans le cadre de l’abonnement. La tarification dans la liste de prix basée sur l’utilisation est organisée autour de différents ID de compteur de ressources dans Azure.

Les réservations Azure sont des achats basés sur des termes pour les machines virtuelles de type de ressource particulier. L’achat d’une réservation Azure permet à un partenaire de prépayer (conditions d’un ou trois ans) et de réserver un ordinateur virtuel donné. Cela permet d’économiser de l’argent partenaire et de s’assurer que leur machine virtuelle est toujours disponible pendant la durée du terme. Un partenaire peut aligner la réservation qu’il souhaite sur les ID de compteur de ressources basés sur l’utilisation. Les ID de compteur sont cohérents au sein de la ressource, que le partenaire achète une machine virtuelle ou déploie simplement la machine virtuelle en tant que ressource basée sur l’utilisation. 


## <a name="offers-matrix"></a>Tableau des offres

Pour plus d’informations sur les références et les offres groupées de produits disponibles à la vente, consultez le tableau des offres des revendeurs cloud de la page Tarification et offres. Le tableau des offres inclut les offres disponibles par région. Si un élément figure dans la liste de prix, mais n’est pas encore répertorié dans le tableau des offres, cela signifie que les produits ne peuvent pas encore être commandés. Dès qu’ils seront disponibles à la commande, le tableau des offres sera mis à jour.

Pour les partenaires CSP qui utilisent les kits de développement logiciel (SDK) de l’espace partenaires. Microsoft publie également une liste des services Azure dans le programme Fournisseur de solutions Cloud dans la page Tarification et offres.

### <a name="offers-matrix-and-pricelist-questions"></a>Questions sur le tableau des offres et la liste de prix

Si vous avez des questions sur la matrice de pricelist ou d’offre, envoyez une demande de service via l’espace partenaires.
