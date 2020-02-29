---
title: Tarification et offres | Espace partenaires
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La liste des offres inclut les différentes familles de produits qui peuvent être achetées via l’espace partenaires et leurs informations de tarification.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e33b89e76a57e1e6f5457e208a61bc04ad841271
ms.sourcegitcommit: 2634057663a0ea27393212f898018538dada796e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/28/2020
ms.locfileid: "78161513"
---
# <a name="pricing-and-offers"></a>Tarification et offres

**S’applique à**

-  Centre pour partenaires

**Rôles appropriés**
-   Administrateur global
-   Administrateur des utilisateurs
-   Agent d’administration
-   Administrateur partenaire MPN
-   Commercial
-   Administration de facturation

Pour voir les derniers programmes du fournisseur de solutions Cloud et les offres, consultez la page **vendre > tarifs et offres**. Vous trouverez des listes de prix distinctes pour les services basés sur des licences, comme Office 365, Microsoft Dynamics CRM et Enterprise Mobility suite, et pour les services basés sur l’utilisation qui incluent Azure. 

La liste des offres inclut les différentes familles de produits qui peuvent être achetées par le biais de l’espace partenaires. Il s’agit actuellement d’Office 365, Enterprise Mobility suite, Microsoft Dynamics CRM et Microsoft Azure. Cette liste continuera à s’étendre à mesure que de nouveaux produits seront disponibles.

Dans chacune de ces familles de produits, vous pouvez vendre différentes références SKU et lots de produits en fonction de votre activité. Vous pouvez toujours accéder aux informations les plus récentes sur ces produits à l’aide de la matrice de l’offre du revendeur Cloud, disponible sur la page tarification et offres.

## <a name="price-list-preview-and-change-frequency"></a>Aperçu de la liste de prix et fréquence des modifications 

Les services basés sur une licence incluent un aperçu de liste de prix, fourni 30 jours à l’avance de toute modification. Pour afficher l’aperçu de la liste de prix, accédez à la page **vendre > tarification et offres**. Aucun aperçu de prix n’est fourni pour les services basés sur l’utilisation, car ces services sont dynamiques. Le tableau suivant explique comment lire la table des tarifs.

|**Élément**        |**Définition**      |
|:-----------   |:-----------   |
|AJOUTER   |Un nouvel élément à la liste de prix|
|CHG   |Modifications du tarif du mois au mois. D’autres modifications non liées au tarif de la liste peuvent se produire, les partenaires doivent comparer les listes de prix entre les mois pour déterminer les modifications apportées aux autres propriétés.|
|DEL   |Un élément a été supprimé de la liste de prix|
|UNC   |Tarif non modifié à partir de la liste de prix du mois précédent  |
|Valide à partir du   |Première date à laquelle une offre peut être commandée    |
|Valide jusqu’au   |Date limite jusqu’à laquelle une offre peut être commandée   |
|Nom d’affichage de l’offre   |Nom de l’offre utilisé pour les clients   |
|ID de l’offre   |Identificateur interne de l’offre   |
|Type de contrat de licence   |Les types de contrat de licence peuvent être Corporate, Government ou Academic et détermine les types de clients pour lesquels l’offre peut être vendue.|
|Unité d’achat   |Il s’agit de la durée de l’offre achetée. Les unités d’achat sont généralement un mois.   |
|Type de licence secondaire   |Les types de licences secondaires sont non spécifiques, complémentaires ou d’essai. Extension indique que le client doit acheter des logiciels requis avant d’acheter l’extension.|
|Type de client final   |Se réfère au type de contrat de licence : licence d’entreprise-revendeur du Cloud-entreprise, licence gouvernementale-gouvernement du revendeur du Cloud ou licence académique-étudiant du Cloud ou de revendeurs de Cloud   |
|Liste de prix   |Prix payé par le partenaire   |
|Prix moyen estimé   |Prix de vente au détail estimé ou recommandé pour le client   |

## <a name="price-changes"></a>Changements de prix

Les changements de prix sont des événements fréquents. Les partenaires peuvent anticiper les changements de prix pour les offres basées sur les licences en regardant la liste de prix dans la page tarification et offres du tableau de bord de l’espace partenaires. La tarification basée sur l’utilisation Azure n’a pas de préversion. Les partenaires peuvent suivre les changements de prix de la consommation Azure à l’aide de l’API RateCard, qui renvoie la tarification du compteur du jour.

|**Type de produit**   |**Exemples de produits**  |**Aperçu disponible** |**Modifier les détails**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basé sur une licence|Office, Dynamics, Intune, Windows entreprise|30 jours|Répertorier les modifications de prix marquées CHNG dans les listes de prix en version préliminaire|
|Basé sur l’utilisation|Ressources Azure|Non disponible|Journal des modifications disponible dans l’onglet **historique des modifications** de la liste de prix du mois précédent|
|Logiciels||Non disponible|Comparer les listes de prix manuellement du mois au mois|
|Les réservations|Machines virtuelles, prépayé|Non disponible|Comparer les listes de prix manuellement du mois au mois|

Les prix basés sur l’utilisation peuvent changer au cours d’un mois. Pour obtenir la tarification quotidienne « actuelle » pour ces ressources Azure, les partenaires doivent appeler l’API RateCard. 

>[!Note] 
>Les changements de prix des abonnements s’appliquent uniquement lors d’un renouvellement. Les frais mensuels d’un partenaire sont déterminés au prix de l’achat ou au prix au moment de la création d’un abonnement. Si un prix augmente ou diminue après l’acquisition du terme annuel, le partenaire ne facture pas le prix modifié jusqu’au renouvellement, généralement à la période de 12 mois.

## <a name="pricing-and-special-segments"></a>Tarification et segments spéciaux

Le fournisseur CSP offre des services à des segments de marché spéciaux, par exemple, l’éducation, le non-bénéfice et le Cloud de la communauté gouvernementale. Tous les services ne sont pas disponibles dans tous les canaux. Aucun segment n’a pour valeur par défaut ce que nous appelons le segment « commercial ». Toutes les tarifs basés sur les licences sont disponibles dans la liste des prix basés sur des licences sur la page tarification et offres. Azure Government tarification est disponible dans la liste de prix basée sur l’utilisation lorsqu’elle est connectée à l’Azure Government locataire CSP activé.

|**Partie**   |**qui doit être qualifié**   |**Le partenaire qualifie le client**|**Types de produits activés**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Éducation|Client|Non, la qualification du client sera effectuée par Microsoft |Basée sur une licence uniquement|
|À but non lucratif|Client|Non, le client répond à l’extérieur de l’espace partenaires|Basée sur une licence uniquement|
|Government Community Cloud (GCC)|Partenaire et client|Une fois que GCC est activé, le partenaire peut créer des clients GCC| Basée sur une licence uniquement|
|Azure gov|Partenaire|Une fois qualifié, le partenaire travaille dans un locataire CSP spécifique à Azure gov|Ressources Azure|

Les marges du partenaire, la différence entre le tarif et les prix estimés au détail, peuvent varier d’un segment à l’autre. En règle générale, l’enseignement et le non-bénéfice ont tendance à avoir des marges inférieures ou égales pour les partenaires CSP. Reportez-vous à la liste des prix basés sur une licence pour obtenir les valeurs exactes.  
## <a name="pricing-between-azure-and-non-azure"></a>Tarification entre Azure et non-Azure

La tarification diffère selon les différents types d’offres. La tarification basée sur les licences est généralement le montant par poste (licence) pour un mois donné. La tarification basée sur l’utilisation est déterminée par l’utilisation d’une ressource donnée, avec un ID de compteur associé. Les partenaires ne sont pas facturés pour l’acquisition de l’abonnement Azure, mais sont facturés pour les ressources consommées par différents déploiements dans le cadre de l’abonnement. La tarification dans la liste de prix basée sur l’utilisation est organisée autour de différents ID de compteur de ressources dans Azure.

Les réservations Azure sont des achats basés sur des termes pour les machines virtuelles de type de ressource particulier. L’achat d’une réservation Azure permet à un partenaire de prépayer (conditions d’un ou trois ans) et de réserver une machine virtuelle donnée, d’enregistrer l’argent partenaire et de s’assurer que la machine virtuelle est toujours disponible pendant la durée du terme. Un partenaire peut aligner la réservation qu’il souhaite sur les ID de compteur de ressources basés sur l’utilisation. Les ID de compteur sont cohérents au sein de la ressource, que le partenaire achète une machine virtuelle ou déploie simplement la machine virtuelle en tant que ressource basée sur l’utilisation. 


## <a name="offers-matrix"></a>Tableau des offres

Pour plus d’informations sur les références et les offres groupées de produits disponibles à la vente, consultez le tableau des offres des revendeurs cloud de la page Tarification et offres. Le tableau des offres inclut les offres disponibles par région. Si un élément figure dans la liste de prix mais pas encore répertorié dans la matrice d’offre, cela signifie que les produits ne peuvent pas encore être commandés. Dès qu’ils seront disponibles à la commande, le tableau des offres sera mis à jour.

Pour les partenaires fournisseurs de solutions Cloud qui utilisent les Kits de développement logiciel (SDK) de l’Espace partenaires. Microsoft publie également une liste des services Azure dans le programme Fournisseur de solutions Cloud dans la page Tarification et offres.

### <a name="offers-matrix-and-price-list-questions"></a>Offre des questions sur les tarifs et la matrice

Si vous avez des questions sur la matrice tarifaire ou offre, envoyez une demande de service via l’espace partenaires.

### <a name="taxes-and-pricing"></a>Taxes et tarification

La tarification des tarifs des fournisseurs de services Cloud est comprise dans les taxes. Pour plus d’informations sur les taxes sur les documents de l’espace partenaires [et](https://docs.microsoft.com/partner-center/tax-and-tax-exemptions)sur les taxes.
