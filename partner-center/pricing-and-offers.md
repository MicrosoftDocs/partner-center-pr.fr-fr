---
title: Tarification et offres
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Consultez les tarifs actuels pour obtenir des services basés sur une licence comme Office 365, Microsoft Dynamics CRM et Enterprise Mobility suite, ainsi que des services basés sur l’utilisation comme Azure.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e92964b2b75a0ee4e9943740ba4da4aa71c82f9f
ms.sourcegitcommit: 3a1c0934ff337fc164bee690e7b9d69d113fdb99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "84328290"
---
# <a name="pricing-and-offers-for-office-365-dynamics-crm-enterprise-mobility-suite-azure-and-more"></a>Tarifs et offres pour Office 365, Dynamics CRM, Enterprise Mobility suite, Azure et bien plus encore

**S’applique à**

- Espace partenaires

**Rôles appropriés**

- Administrateur général
- Administrateur des utilisateurs
- Agent d’administration
- Administrateur partenaire MPN
- Agent commercial
- Administrateur de la facturation

Pour afficher les derniers programmes et offres de fournisseurs de solutions Cloud, à partir du portail partenaires, accédez à la page **vendre > tarification et offres**. Vous trouverez des listes de prix distinctes pour les services basés sur les licences, notamment Office 365, Microsoft Dynamics CRM et Enterprise Mobility suite, ainsi que pour les services basés sur l’utilisation qui incluent Azure.

La liste des offres inclut les différentes familles de produits qui peuvent être achetées par le biais de l’espace partenaires. Il s’agit actuellement d’Office 365, Enterprise Mobility suite, Microsoft Dynamics CRM et Microsoft Azure. Cette liste continuera à s’étendre à mesure que de nouveaux produits seront disponibles.

Dans chacune de ces familles de produits, vous pouvez vendre différentes références SKU et lots de produits en fonction de votre activité. Vous pouvez toujours accéder aux informations les plus récentes sur ces produits à l’aide de la matrice de l’offre du revendeur Cloud, disponible sur la page tarification et offres.

## <a name="price-list-preview-and-change-frequency"></a>Aperçu de la liste de prix et fréquence des modifications 

Les services basés sur une licence incluent un aperçu de liste de prix, fourni 30 jours à l’avance de toute modification. Pour afficher l’aperçu de la liste de prix, accédez à la page **vendre > tarification et offres**. Il n’existe pas d’aperçu des prix pour les services basés sur l’utilisation, car ces services sont dynamiques. Le tableau suivant explique comment lire la table des tarifs.

|**Item**        |**Définition**      |
|:-----------   |:-----------   |
|ADD   |Un nouvel élément à la liste de prix|
|CHANGEMENTS   |Modifications du tarif du mois au mois. D’autres modifications non liées au tarif de la liste peuvent se produire, les partenaires doivent comparer les listes de prix entre les mois pour déterminer les modifications apportées aux autres propriétés.|
|DEL   |Un élément a été supprimé de la liste de prix|
|UNC   |Tarif non modifié à partir de la liste de prix du mois précédent  |
|Date de validation valide   |La première date à laquelle une offre peut être commandée    |
|Date de validité   |Dernière date à laquelle une offre peut être commandée   |
|Nom complet de l’offre   |Nom du client pour l’offre   |
|ID de l’offre   |Identificateur interne de l’offre   |
|Type de contrat de licence   |Les types de contrat de licence peuvent être Corporate, Government ou Academic. Le type d’accord détermine les types de clients pour lesquels l’offre peut être vendue.|
|Unité d’achat   |Durée de l’achat de l’offre. Les unités d’achat sont généralement un mois.   |
|Type de licence secondaire   |Les types de licences secondaires sont non spécifiques, complémentaires ou d’essai. Le module complémentaire indique qu’il existe des produits prérequis que le client doit acheter avant d’acheter le module complémentaire.|
|Type de client final   |Se réfère au type de contrat de licence : licence d’entreprise-revendeur du Cloud-entreprise, licence gouvernementale-gouvernement du revendeur du Cloud ou licence académique-étudiant du Cloud ou de revendeurs de Cloud   |
|Tarif   |Le prix payé par le partenaire   |
|Prix ERP   |Prix de vente estimé ou recommandé au client   |

## <a name="price-changes"></a>Changements de prix

Les changements de prix sont des événements fréquents. Les partenaires peuvent anticiper les changements de prix pour les offres basées sur les licences en regardant la liste de prix en préversion. Dans le tableau de bord de l’espace partenaires, ouvrez la page tarification et offres pour afficher l’aperçu de la liste de prix.

Toutefois, la tarification basée sur l’utilisation Azure n’a pas d’aperçu. Les partenaires peuvent suivre les changements de prix de la consommation Azure à l’aide de l’API RateCard, qui renvoie la tarification du compteur du jour.

|**Type de produit**   |**Exemples de produits**  |**Aperçu disponible** |**Détails des modifications**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basé sur une licence|Office, Dynamics, Intune, Windows entreprise|30 jours|Répertorier les modifications de prix marquées CHNG dans les listes de prix en version préliminaire|
|Basé sur l’utilisation|Ressources Azure|Non disponible|Journal des modifications disponible dans l’onglet **historique des modifications** de la liste de prix du mois précédent|
|Logiciel||Non disponible|Comparer les listes de prix manuellement du mois au mois|
|Réservations|Machines virtuelles, prépayé|Non disponible|Comparer les listes de prix manuellement du mois au mois|

Les prix basés sur l’utilisation peuvent changer au cours d’un mois. Pour obtenir la tarification quotidienne « actuelle » pour ces ressources Azure, les partenaires doivent appeler l’API RateCard. 

> [!Note] 
> Les changements de prix des abonnements s’appliquent uniquement lors d’un renouvellement. Les frais mensuels d’un partenaire sont déterminés au prix de l’achat ou au prix au moment de la création d’un abonnement. Si un prix augmente ou diminue après l’acquisition du terme annuel, le partenaire ne facture pas le prix modifié jusqu’au renouvellement, généralement à la période de 12 mois.

## <a name="pricing-and-special-segments"></a>Tarification et segments spéciaux

Le fournisseur CSP offre des services à des segments de marché spéciaux, par exemple, l’éducation, le non-bénéfice et le Cloud de la communauté gouvernementale. Tous les services ne sont pas disponibles dans chaque canal. Aucun segment n’a pour valeur par défaut ce que nous appelons le segment « commercial ». Toutes les tarifs basés sur les licences sont disponibles dans la liste des prix basés sur des licences sur la page tarification et offres. Azure Government tarification est disponible dans la liste de prix basée sur l’utilisation lorsqu’elle est connectée à l’Azure Government locataire CSP activé.

|**Segment**   |**qui doit être qualifié**   |**Le partenaire qualifie le client**|**Types de produits activés**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Formation|Customer|Non, la qualification du client sera effectuée par Microsoft |Basée sur une licence uniquement|
|À but non lucratif|Customer|Non, le client répond à l’extérieur de l’espace partenaires|Basée sur une licence uniquement|
|Government Community Cloud (GCC)|Partenaire et client|Une fois que GCC est activé, le partenaire peut créer des clients GCC| Basée sur une licence uniquement|
|Azure Government|Partenaire|Une fois qualifié, le partenaire travaille dans un locataire CSP spécifique à Azure Government|Ressources Azure|

Les marges du partenaire, la différence entre le tarif et les prix estimés au détail, peuvent varier d’un segment à l’autre. En règle générale, l’enseignement et le non-bénéfice ont tendance à avoir des marges inférieures ou égales pour les partenaires CSP. Reportez-vous à la liste des prix basés sur une licence pour obtenir les valeurs exactes.  
## <a name="pricing-between-azure-and-non-azure"></a>Tarification entre Azure et non-Azure

La tarification diffère selon les différents types d’offres. La tarification basée sur les licences est généralement le montant par poste (licence) pour un mois donné. La tarification basée sur l’utilisation est déterminée par l’utilisation d’une ressource donnée, avec un ID de compteur associé. Les partenaires ne sont pas facturés pour l’acquisition de l’abonnement Azure. Toutefois, les partenaires sont facturés pour les ressources consommées par différents déploiements dans le cadre de l’abonnement Azure. La tarification dans la liste de prix basée sur l’utilisation est organisée autour de différents ID de compteur de ressources dans Azure.

Les réservations Azure sont des achats basés sur des termes pour les machines virtuelles de type de ressource particulier. L’achat d’une réservation Azure permet à un partenaire de prépayer (conditions d’un ou trois ans) et de réserver un ordinateur virtuel donné. Les réservations enregistrent l’argent du partenaire et s’assurent que leur machine virtuelle est toujours disponible pendant la durée du terme. Un partenaire peut aligner la réservation qu’il souhaite sur les ID de compteur de ressources basés sur l’utilisation. Les ID de compteur sont cohérents au sein de la ressource, que le partenaire achète une machine virtuelle ou déploie simplement la machine virtuelle en tant que ressource basée sur l’utilisation.

## <a name="offers-matrix"></a>Matrice des offres

Sur la page tarification et offres, consultez la matrice de l’offre du revendeur Cloud pour en savoir plus sur les différentes références SKU et les offres groupées disponibles pour la vente. La matrice offres inclut les offres disponibles par paramètres régionaux. Si un élément est répertorié dans la liste de prix mais pas dans la matrice d’offre, cela signifie que les produits ne peuvent pas encore être commandés. Dès qu’elles sont disponibles pour la commande, la matrice offres est mise à jour.

Pour les partenaires CSP qui utilisent les kits de développement logiciel (SDK) de l’espace partenaires. Microsoft publie également une liste des services Azure dans CSP sur la page tarification et offres.

### <a name="offers-matrix-and-price-list-questions"></a>Offre des questions sur les tarifs et la matrice

Si vous avez des questions sur la matrice tarifaire ou offre, envoyez une demande de service via l’espace partenaires.

## <a name="offer-limits"></a>Limites de l’offre

Certaines offres basées sur une licence présentent certaines règles et limitations qui interdisent l’achat de plusieurs achats pour le même client. Ces règles s’appliquent à la plupart des versions d’évaluation et à la plupart des petites offres commerciales. Les **offres Small Business** sont définies par les offres qui ont un nombre de licences maximal inférieur à 300.

Ces contraintes d’achat sont définies dans le cadre de la configuration de l’offre et peuvent être trouvées en consultant la matrice liste des offres. Deux colonnes de données fonctionnent ensemble pour définir la mise en application : 1. Étendue de limite d’offre et 2. Limite de l’offre. Les contraintes sont appliquées au cours d’un achat. Dans l’espace partenaires, le catalogue interdit à un partenaire d’acheter plus d’offres que les règles n’autorisent. Toute tentative de violation des contraintes entraînera une erreur.

L’étendue de la limite d’offre est enregistrée sous la forme d’une colonne dans la matrice liste d’offres et peut avoir les valeurs aucune, durée de vie ou simultanée. 

- Les offres avec **aucune** peuvent être achetées sans contraintes.
- Les offres de **durée de vie** ne peuvent être achetées qu’une seule fois.
- Les offres **simultanées** peuvent être achetées autant de fois que le nombre autorisé par la valeur **limite d’offre** pour cette offre. La plupart des essais ont une étendue de durée de vie limitée avec une limite d’offre de « 1 ». La plupart des offres de petite entreprise ont une étendue de limite d’offre simultanée avec une limite de « 2 ».

> [!IMPORTANT]
> Les limites de concurrence sont appliquées même si une offre est annulée. Une offre doit être complètement annulée, puis annulée pour libérer de l’espace supplémentaire, ce qui permet d’obtenir un autre achat.

### <a name="taxes-and-pricing"></a>Taxes et tarification

La tarification des tarifs des fournisseurs de services Cloud est comprise dans les taxes. Pour plus d’informations sur les taxes sur les documents de l’espace partenaires [et](tax-and-tax-exemptions.md)sur les taxes.
