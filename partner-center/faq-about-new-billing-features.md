---
title: "FAQ sur les nouvelles fonctionnalités de facturation| Espace partenaires"
Description: The following are frequently asked questions about Partner Center's annual billing and free trial features.
author: MaggiePucciEvans
ms.openlocfilehash: 503a1fac539b2cd40e8b95ab458143801c5d0134
ms.sourcegitcommit: 4964383ea9dcd51d27256a2969a453d67c5ebf0c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/03/2018
---
# <a name="faq-about-new-billing-features"></a>FAQ sur les nouvelles fonctionnalités de facturation

**S'applique à**

-  Espace partenaires
-  Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis
-  Espace partenaires de MicrosoftCloud Germany

Vous trouverez ci-dessous les réponses aux questions fréquemment posées à propos de la facturation annuelle et des essais gratuits de l'Espace partenaires. 

## <a name="in-this-section"></a>Dans cette section

-   [FAQ sur la facturation annuelle](#annualbillingfaq)

-   [FAQ sur les essais gratuits](#freetrialsfaq)

-   [FAQ sur l'ajustement des dates de facturation](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>FAQ sur la facturation annuelle

Sections:

[Présentation et avantages de la facturation annuelle](#overviewandbenefits)

[Processus de commande et scénarios de facturation](#placingyourorder)

[Modification de votre abonnement](#changingyoursubscription)

[Calcul des tarifs](#pricingcalculation)

[Rapports](#reporting)

[Primes incitatives](#incentives)


<a href="" id="overviewandbenefits"></a>**Présentation et avantages de la facturation annuelle**

**Q:** Quels sont les changements?

-   **R:** En réponse à vos demandes, nous avons introduit la possibilité de régler certains abonnements CSP une fois par an ou une fois par mois. Cette nouvelle option sera disponible le 17octobre2017.

**Q:** Qui peut participer?

-   **R:** Tous les partenaires de tous types peuvent bénéficier d'une facturation annuelle. La facturation annuelle est disponible dans tous les marchés où le programme Fournisseur de solutions Cloud est actuellement disponible. 

**Q:** Que dois-je prendre en considération pour envisager une facturation annuelle?    

-   **R:** Vous devez réfléchir à son incidence sur votre proposition de vente. Voici quelques conseils pour vous aider à utiliser efficacement la facturation annuelle. 
    - Mettez à jour les API pour prendre en compte la fonctionnalité de facturation annuelle, le cas échéant. 
    - Examinez les modifications apportées à la facture et au fichier de rapprochement basé sur les licences.
    - Assurez-vous que votre équipe est informée.
    - Mettez à jour vos processus internes si nécessaire.

**Q:** Quels sont les avantages de la facturation annuelle? 

-   **R:** La facturation annuelle présente les avantages suivants:

    - Flexibilité accrue en matière d'options de paiement.

    - Meilleur alignement avec la facturation de vos clients.

    - Réduction de l'impact des fluctuations de devises.

    - Réduction des coûts d'exploitation en matière de facturation.

**Q:** Quelles sont les offres qui proposent l'option de facturation annuelle?

-   **R:** La plupart des abonnements basés sur la licence proposent une facturation mensuelle ou annuelle. Les abonnements basés sur l'utilisation proposent uniquement une facturation mensuelle. Vous pouvez consulter les fréquences de facturation disponibles pour chaque offre dans la colonneJ du tableau des offres. Vous trouverez le tableau des offres dans la section «Voir les offres et leur tarification» de l'Espace partenaires. .

**Q:** S'agit-il d'une facturation annuelle par abonnement ou par licence?       

-   **R:** Les facturations annuelle et mensuelle s'appliquent par abonnement.

**Q:** Est-il nécessaire de modifier les API pour prendre en charge la facturation annuelle?    

-   **R:** Pour tirer parti de la facturation annuelle, certaines modifications de vos API sont nécessaires. Vous trouverez plus d'informations dans les articles suivants:

    - https://partnercenter.microsoft.com/fr-fr/partner/developer

    - https://msdn.microsoft.com/fr-fr/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Exemple de code: https://msdn.microsoft.com/fr-fr/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Processus de commande et scénarios de facturation**

**Q:** Une offre unique sera-t-elle proposée spécialement pour les commandes avec facturation annuelle?   

-   **R:** Non. Toutes les fréquences de facturation, y compris l'option de facturation annuelle, sont affectées à l'offre sous forme d'attribut. Toutefois, vous pouvez donner à une offre un nom plus explicite pour aider les clients à faire facilement la distinction.

**Q:** Comment sélectionner la facturation annuelle?

-   **R:** Lorsque vous ajoutez un nouvel abonnement, vous devez choisir sa fréquence de facturation. Vous pouvez choisir l'option de facturation annuelle à ce stade. Une fois la facturation annuelle sélectionnée, toutes les offres disponibles s'affichent.

**Q:** Si j'opte pour la facturation annuelle, quand serai-je facturé?    

-   **R:** Vous serez facturé à la date de facturation suivante. Par exemple, si votre date de facturation est le 1erfévrier, vous serez toujours facturé le 1erfévrier. Par conséquent, si vous achetez un abonnement à facturation annuelle le 29octobre2017 ou le 15janvier2018, dans les deux cas, la date de facturation sera le 1erfévrier2018. 

**Q:** Puis-je diviser un abonnement pour qu'une partie soit facturée une fois par mois et l'autre une fois par an?  

-   **R:** Non. L'intégralité de l'abonnement doit avoir la même fréquence de facturation. L'intégralité de l'abonnement doit donner lieu à une facturation mensuelle ou annuelle.

**Q:** Quelle est la date de renouvellement d'un abonnement à facturation annuelle?     

-   **R:** La date de renouvellement est fixée à 12mois après la date de démarrage du service. La période de service commence à la date de création de l'abonnement.  Par exemple, un abonnement créé le 10janvier2018 sera renouvelé le 10janvier2019.

**Q:** Quand serai-je facturé pour le renouvellement d'un abonnement à facturation annuelle? 

-   **R:** Vous serez facturé à la prochaine date de facturation qui suit la date de renouvellement de l'abonnement. Par exemple, si vous achetez un abonnement à facturation annuelle le 15janvier2018 et que votre date de facturation est le 20janvier, votre abonnement sera renouvelé le 15janvier2019. Vous serez facturé pour le renouvellement le 20janvier2019.

**Q:** Les abonnements à facturation annuelle bénéficient-ils d'une période gratuite?

-   **R:** Non, les abonnements à facturation annuelle ne font pas l'objet d'une période gratuite. La période d'abonnement de 12mois commence à la date d'achat. Ces conditions diffèrent de celles des abonnements à fréquence de facturation mensuelle qui bénéficient d'une période gratuite entre la date d'achat et la date de facturation qui suit.

**Q:** Un client peut-il avoir plusieurs abonnements pour une même offre, chacun avec une fréquence de facturation différente?    

-   **R:** Cela dépend de l'offre. Certaines offres sont limitées à un abonnement par client. Si l'offre n'est pas limitée, un client peut avoir plusieurs abonnements d'une même offre avec des fréquences de facturation différentes. Vous trouverez les détails des limites et restrictions de chaque offre dans la colonneI du tableau des offres. Vous trouverez le tableau des offres dans la section «Voir les offres et leur tarification» de l'Espace partenaires.

<a href="" id="changingyoursubscription"></a>**Modification de votre abonnement**

**Q:** Puis-je ajouter une nouvelle licence à un abonnement existant faisant l'objet d'une facturation annuelle?    

-   **R:** Oui. Vous pouvez modifier le nombre de licences de vos abonnements à tout moment. L'ajout de licences supplémentaires n'aura aucune incidence sur la fréquence de facturation. 

**Q:** Puis-je ajouter des licences donnant lieu à une facturation mensuelle à un abonnement existant faisant l'objet d'une facturation annuelle? 

-   **R:** Une fois que vous achetez un abonnement à facturation annuelle, toutes les licences supplémentaires respecteront la même fréquence de facturation. Si par la suite vous devez acheter des licences à facturation mensuelle, vous devrez acheter un nouvel abonnement.

**Q:** Puis-je passer la fréquence de facturation d'un abonnement de mensuelle à annuelle et vice versa? 

-   **R:** Non. Une fois que vous avez sélectionné la fréquence de facturation, vous ne pouvez pas la modifier. 

**Q:** La facturation annuelle est-elle disponible pour les offres de module complémentaire?   

-   **R:** Oui. L'abonnement au module complémentaire aura automatiquement la même fréquence de facturation que l'abonnement parent.

**Q:** Comment fonctionnera la facturation annuelle si j'ajoute ou supprime des licences? 

-   **R:** Vous pouvez à tout moment ajouter ou supprimer des licences. Vous recevrez un crédit et une refacturation au prorata lors de la prochaine date de facturation qui suit la modification du nombre de licences. 

**Q:** Que se passe-t-il si j'annule un abonnement à facturation annuelle?    

-   **R:** La politique d'annulation est la même pour toutes les fréquences de facturation. Si l'abonnement est supprimé dans les 30premiers jours de la période payante de 12mois, vous recevrez un crédit de 100% à la date de facturation suivante. Si l'abonnement est annulé 30jours après le début de la période d'abonnement de 12mois, vous serez crédité au prorata à la date de facturation suivante.

**Q:** Un client peut-il transférer un abonnement à facturation annuelle d'un partenaire à un autre?  

-   **R:** Non. Les abonnements ne peuvent pas être transférés entre des partenaires. Le nouveau partenaire doit acheter un nouvel abonnement pour le compte du client. Cela s'applique aussi bien aux abonnements à facturation mensuelle qu'annuelle.

**Q:** Puis-je réactiver un abonnement à facturation annuelle?

-   **R:** Oui, vous pouvez réactiver l'abonnement jusqu'à 90jours à partir de la date de suspension. Les frais calculés au prorata seront facturés à la date de facturation suivante. La date de renouvellement de l'abonnement reste identique.

<a href="" id="pricingcalculation"></a>**Calcul des tarifs**

**Q:** Que se passe-t-il si le prix d'une offre change au cours de la période de 12mois d'un abonnement à facturation annuelle?    

-   **R:** Le prix de l'offre au moment de l'achat est garanti pour toute la période de 12mois de l'abonnement. 

**Q:** À quel prix sera l'abonnement à son renouvellement automatique au bout des 12mois d'abonnement?    

-   **R:** Lors du renouvellement d'un abonnement, le prix est basé sur la liste des prix en vigueur à la date du renouvellement. Le nouveau prix est garanti pour la période des 12mois suivants de l'abonnement.

**Q:** Comment le crédit pour l'annulation d'une licence ou d'un abonnement est-il calculé? Est-il calculé à la journée ou au mois?   

-   **R:** Le crédit d'annulation est calculé comme suit:

    - Crédit d'annulation = ((prix mensuel*12)/365) * nombre de jours restants dans la période de 12mois * nombre de licences annulées.

**Q:** Que se passe-t-il si le prix d'une offre diminue au cours de la période de 12mois d'un abonnement à facturation annuelle? 

-   **R:** Cela ne change rien. Le prix est défini pour toute la période de 12mois. Il en va de même pour une facturation mensuelle.


<a href="" id="reporting"></a>**Rapports**

**Q:** Comment savoir si un abonnement est facturé chaque année ou tous les mois?   

-   **R:** Le fichier de rapprochement basé sur la licence contient des informations sur la fréquence de facturation. Vous les trouverez dans la colonne AA

**Q:** Quelles modifications apparaissent dans le fichier de rapprochement basé sur la licence lors de l'achat ou du renouvellement d'un abonnement à facturation annuelle?  

-   **R:** La première modification consiste en une nouvelle ligne dans le fichier de rapprochement basé sur la licence lors de la première date de facturation qui suit un achat ou un nouvel abonnement. . Si aucune modification n'est apportée à l'abonnement, aucune ligne n'apparaît sur les fichiers de rapprochement pour les mois2 à 12 de la période d'abonnement. La prochaine modification apportée au fichier de rapprochement s'affiche lors du renouvellement de l'abonnement. Elle s'affiche à la première date de facturation qui suit le renouvellement. Si une modification est apportée à l'abonnement au cours de la période de 12mois, un crédit et une refacturation au prorata apparaîtront sur le prochain fichier de rapprochement qui suit la modification.

**Q:** Comment apparaît l'achat, la modification ou l'annulation d'un abonnement annuel dans la colonneP des fichiers d'utilisation?

-   **R:** Les frais d'achat initiaux apparaissent sous forme de «frais au prorata à l'achat». Les modifications de licence qui font l'objet d'un crédit et d'une refacturation s'affichent sous forme d'«Instance de cycle au prorata». Les crédits d'annulation apparaissent sous forme de «Frais d'annulation».

**Q:** Lorsqu'un abonnement annuel est annulé, comment cela apparaît-il sur le fichier de rapprochement?   

-   **R:** Le fichier de rapprochement contient une ligne indiquant un crédit d'annulation. Si l'annulation se produit dans les 30premiers jours de la période de 12mois, l'abonnement sera crédité à 100%. Si l'annulation se produit après les 30premiers jours, l'abonnement sera crédité au prorata.

**Q:** Comment l'ajout de licences à un abonnement à facturation annuelle apparaît-il sur le fichier de rapprochement?  

-   **R:** Le fichier de rapprochement contient un crédit et une refacturation au prorata. C'est également le cas pour un abonnement à facturation mensuelle.

**Q:** Comment la suppression de licences d'un abonnement à facturation annuelle apparaît-elle sur le fichier de rapprochement? 

-   **R:** Le fichier de rapprochement contient un crédit et une refacturation au prorata.  C'est également le cas pour un abonnement à facturation mensuelle.

**Q:** Le prix annuel est-il indiqué sur la liste de prix? 

-   **R:** Non. La liste de prix indique le prix mensuel. Vous pouvez calculer le prix annuel en multipliant le prix mensuel par douze.

**Q:** Le tableau des offres indique-t-il des entrées différentes pour les offres qui peuvent être facturées annuellement?   

-   **R:** Non. Les identifiants des offres sont les mêmes pour toutes les fréquences de facturation. Il n'existe pas d'identifiant unique pour les offres à facturation annuelle.


<a href="" id="incentives"></a>**Primes incitatives**

**Q:** À quelle fréquence les primes incitatives sont-elles calculées sur les abonnements annuels? 

-   **R:** Nous les calculons sur les revenus facturés. Les paiements des primes obtenues seront versés conformément à notre stratégie présentée dans les guides de primes incitatives de notre programme Fournisseur de solutions Cloud. 

**Q:** Comment les primes incitatives sur les abonnements à facturation annuelle sont-elles payées?  

-   **R:** À présent, tous les paiements des primes incitatives sont effectués deux fois par an. Ces paiements sont versés 45jours après la fin du semestre.

**Q:** Lorsqu'un abonnement à facturation annuelle est vendu, comment les revenus de cet abonnement sont-ils pris en compte pour le calcul des primes incitatives? Le calcul est-il basé sur les revenus payés ou ajustés? 

-   **R:** Le calcul des primes incitatives est basé sur les revenus facturés.

**Q:** Comment les bénéfices des primes incitatives sur les abonnements à facturation annuelle éligibles sont-ils calculés parmi les différents taux de primes du programme Fournisseur de solutions Cloud (taux de primes mondiaux, taux accélérateurs locaux et campagnes locales)?

-   **R:** Quel que soit le mode de facturation (mensuel ou annuel) de l'abonnement, les partenaires gagnent des primes incitatives sur toutes les transactions éligibles. Cela inclut le taux de prime mondial, appliqué au revenu facturé pour la période, l'accélérateur local pour toutes les régions où il existe des accélérateurs locaux et les campagnes mondiales, le cas échéant.

**Q:** Qui contacter pour répondre aux questions sur les primes incitatives?

-   **R:** Contactez l'équipe de support régionale appropriée pour les primes incitatives:

    - Amérique du Nord: ocina@microsoft.com

    - Amérique latine et Brésil: ocilatam@microsoft.com

    - EMEA: ociemea@microsoft.com

    - APOAC (à l'exception du Japon): ociapgc@microsoft.com

    - Japon: ocijp@microsoft.com


**Q:** Que se passe-t-il si je suspends mon abonnement? 

-   **R:** Si vous suspendez un abonnement dans l'Espace partenaires ou via l'API, dans les 30jours suivant l'achat, vous recevrez un crédit de 100%, quelle que soit la fréquence de facturation. 

    Avec une facturation annuelle, cela se présenterait comme suit:

    - Achat par le partenaire d'un abonnement le 1erjanvier=création d'une ligne de facturation de frais pour la période de service du 01/01 au 31/12.
    - Suspension de l'abonnement le 25janvier=création d'une ligne de facturation de crédit pour la période de service du 01/01 au 31/12.
    - Réactivation le 29janvier=création d'une ligne de facturation de frais pour la période de service du 29/01 au 31/12.

    Avec une facturation mensuelle, cela se présenterait comme suit:

    - Achat par le partenaire d'un abonnement le 1erjanvier=création d'une ligne de facturation de frais pour la période de service du 01/01 au 31/12.
    - Suspension de l'abonnement le 25janvier=création d'une ligne de facturation de crédit pour la période de service du 01/01 au 31/01.
    - Réactivation le 29janvier=création d'une ligne de facturation de frais pour la période de service du 29/01 au 31/01.



## <a href="" id="freetrialsfaq"></a>FAQ sur les essais gratuits

**Q:** En quoi consiste les essais gratuits?

-   **R:** Vous pouvez proposer à vos clients un essai gratuit de certains produits pendant 30jours. Cela leur permet d'évaluer le produit avant de l'acheter. Des essais gratuits sont proposés pour les produits suivants: 

    - Office365 Business Premium  
    - Office365E3  
    - Office365E5 avec PSTN  
    - Office365E5 sans PSTN  
    - EnterpriseMobility+ Security E5  
    - Formule Dynamics365 Customer Engagement1  
    - Dynamics365 for Financials  
    
**Q:** La période gratuite est-elle supprimée avec les essais gratuits?

-   **R:** Non, les abonnements à facturation mensuelle continueront de bénéficier d'une période gratuite. Toutefois, il n'y aura aucune période gratuite pour la facturation annuelle.

**Q:** L'ajustement des dates de facturation a été reporté au 1ertrimestre de l'exercice fiscal2018. Quel est l'impact sur la période gratuite et la facturation en général?

-   **R:** Les nouveaux abonnements à facturation mensuelle continueront de bénéficier d'une période gratuite et de s'aligner sur la date de facturation du partenaire. Les abonnements à facturation annuelle ne proposeront pas de période gratuite et s'aligneront sur la date d'achat. Les partenaires continueront de recevoir leurs fichiers de facture et de rapprochement à la date de facturation mensuelle, ce qui leur permettra de consulter l'activité de facturation des abonnements mensuels et annuels.

**Q:** À quel moment la période gratuite sera-t-elle supprimée pour les abonnements avec une fréquence de facturation mensuelle?

-   **R:** Au 1ertrimestre de l'année fiscale 2018.

**Q:** La facturation annuelle et les essais gratuits sont-ils différents dans le cloud souverain et le cloud public?

-   **R:** Non. Ils sont identiques. La seule différence réside dans les références d'évaluation qui sont disponibles au moment du lancement.

**Q:** Quand celles-ci seront-elles disponibles pour les références répertoriées ci-dessus?

-   **R:** 17octobre2017.

**Q:** Qui peut participer?

-   **R:** Tous les partenaires peuvent participer. Toutefois, ce n'est pas actuellement disponible en Chine. Les essais gratuits seront disponibles pour les clients et partenaires chinois avant la fin de 2017. 

**Q:** Quelles mesures dois-je prendre pour pouvoir bénéficier de ces essais gratuits?

-   **R:** Déterminez la manière dont l'essai gratuit peut être intégré à vos propositions de vente et l'impact sur vos processus internes. Vous devrez peut-être également modifier vos API pour prendre en charge la conversion d'un essai gratuit en abonnement payant. Des spécifications techniques détaillées pour les modifications apportées aux API sont présentées dans la vue Annonces de l'Espace partenaires.

**Q:** L'essai gratuit apparaîtra-t-il dans ma facture et dans le fichier de rapprochement?

-   **R:** Non, les essais gratuits n'apparaissent pas dans votre facture ou votre fichier de rapprochement basé sur la licence. Ils apparaîtront dans votre facture et votre fichier de rapprochement basé sur la licence une fois que vous les aurez convertis en abonnements payants. Un abonnement converti s'affiche à la fois sur votre facture et sur votre fichier de rapprochement basé sur la licence, de la même manière qu'un nouvel abonnement.

**Q:** Les essais gratuits ont-ils un impact sur les primes incitatives?

-   **R:** Non. L'essai gratuit n'aura aucun impact sur les primes.

**Q:** Des essais gratuits seront-ils proposés ultérieurement pour d'autres produits Office et du programme Fournisseur de solutions Cloud?

-   **R:** Nous ne le savons pas encore. Nous fournissons des essais gratuits pour ces produits, parce qu'il s'agit des offres commerciales les plus complètes et les plus populaires. Il se peut que nous ajoutions d'autres offres d'essais gratuits à l'avenir.

**Q:** Un client peut-il bénéficier de plusieurs essais gratuits?

-   **R:** Chaque client a droit à un essai gratuit par offre disponible.

**Q:** L'essai gratuit est-il limité?

-   **R:** Oui. L'essai est valable pour un maximum de 25licences. Le nombre de licences ne peut pas être modifié pendant la période d'essai. Une fois l'essai converti en abonnement payant, vous pouvez lui ajouter des licences supplémentaires.

**Q:** L'essai gratuit est-il automatiquement converti en abonnement payant?

-   **R:** Non. Vous devez convertir l'abonnement vous-même, dans l'Espace partenaires ou via l'API.

**Q:** Les essais gratuits peuvent-ils être utilisés aussi bien pour des abonnements à facturation mensuelle qu'annuelle?

-   **R:** Oui. Vous choisissez la fréquence de facturation lorsque vous convertissez l'essai en abonnement payant.

**Q:** La date de début de l'abonnement sera-t-elle basée sur la date de début de l'essai gratuit ou sur la date de sa conversion en abonnement payant? 

-   **R:** La date de début est basée sur la date de conversion. Si l'essai gratuit est converti en offre payante à facturation annuelle, la date de renouvellement de l'abonnement sera 12mois à compter de la date de conversion. Si l'essai gratuit est converti en une offre payante avec facturation mensuelle, la date de renouvellement de l'abonnement sera 12mois à compter de la date de facturation suivant la date de conversion.

**Q:** Pouvons-nous ajouter ou supprimer des licences pendant l'essai gratuit?

-   **R:** Non. Le nombre de licences par défaut pour les essais gratuits sera égal à 25 et ne pourra pas être modifié.

**Q:** Existe-t-il des essais pour des offres de module complémentaire comme ATP et PSTN?

-   **R:** Il n'existe aucun essai gratuit pour les offres de module complémentaire.

**Q:** Puis-je proposer un essai gratuit pour une offre qu'un client possède déjà?

-   **R:** Non. Si le client possède déjà l'offre, elle ne peut pas être utilisée pour un essai gratuit.

**Q:** Pourrai-je consulter toutes mes offres d'essai gratuit en attente?

-   **R:** Oui. La page du client répertorie tous les abonnements. Elle indique à la fois les abonnements d'essai gratuit et les abonnements payants.

**Q:** Serai-je averti de l'arrivée à expiration des essais gratuits?

-   **R:** Non. Vous pouvez suivre les dates d'expiration à venir soit à l'aide de la vue des clients dans l'Espace partenaires, soit en interrogeant l'API. Il est recommandé de contrôler fréquemment ces dates afin de pouvoir prendre les mesures de suivi appropriées auprès des clients à l'approche du moment où ils doivent prendre une décision.

**Q:** Si un client bénéficie déjà d'un essai gratuit pour une offre, peut-il également utiliser un autre essai pour une autre offre? 

-   **R:** Oui. Les clients peuvent souscrire un essai par offre. Par exemple, ils peuvent obtenir un essai gratuit pour Office365 Business Premium et un autre pour Office365E3.

**Q:** Que se passe-t-il lorsque l'essai se termine? Mon client ou moi allons-nous recevoir une notification? Quelles notifications apparaissent-elles lors d'une tentative de connexion à un essai arrivé à expiration?

-   **R:** Une fois l'essai terminé, un message indiquant que l'essai est arrivé à expiration s'affiche quand le client tente de s'y connecter. Aucune notification ne sera mise en place pour indiquer qu'un essai arrive à expiration, mais en tant que partenaire, vous pouvez en assurer le suivi en consultant la vue des clients ou par l'intermédiaire de requêtes à l'API.

**Q:** Un essai peut-il être prolongé?

-   **R:** Non. Au bout de 30jours, l'essai doit être converti, sinon, il expirera.

**Q:** Lorsqu'un essai expire, les informations qu'il contient sont-elles accessibles?

-   **R:** Oui. Les données sont stockées conformément aux normes de conservation des données. Dès que vous achetez un nouvel abonnement avec les mêmes plans de service, les données sont accessibles à partir de l'abonnement qui vient d'être activé.

**Q:** Les essais gratuits sont-ils disponibles pour les offres Secteur Public et Éducation?

-   **R:** Aucun essai gratuit n'est proposé pour les offres Secteur Public et Éducation pour l'instant.

**Q:** Les essais gratuits d'un client pour le programme Fournisseur de solutions Cloud peuvent-ils être convertis en d'autres clients de programme comme EA, Open ou MOSP? 

-   **R:** Non. Les abonnements ne peuvent pas être transférés du programme Fournisseur de solutions Cloud vers un autre programme.

**Q:** Comment puis-je obtenir un support sur les essais gratuits? 

-   **R:** Veuillez soumettre une demande de service via l'Espace partenaires.

## <a href="" id="billingalignmentfaq"></a>Ajustement de la facturation - Fin de la période gratuite

Le 20février, le programme Fournisseur de solutions Cloud mettra en œuvre l'«ajustement des dates de facturation» pour les nouveaux abonnements avec une fréquence de facturation mensuelle. Cet «ajustement des dates de facturation» donnera une plus grande flexibilité aux partenaires ainsi qu'une meilleure prévision de leurs ventes et de leur facturation. Il permettra en outre d'améliorer l'approvisionnement et la gestion des abonnements des clients. Les abonnements achetés avant le 20février bénéficieront d'une période gratuite allant de la date de l'achat à la date de facturation du partenaire. Les abonnements achetés après le 20février ne bénéficieront plus d'une période gratuite. La période payante de douze mois démarrera (s'ajustera) à la date d'achat au lieu de la date de facturation du partenaire. Les partenaires ne verront plus la ligne «Facturation 0» qui représente la période de gratuité sur le fichier de rapprochement. Aucune modification n'est apportée aux API de facturation ou aux primes incitatives.  Les partenaires doivent informer leurs équipes de vente et de gestion des comptes de cette nouvelle logique de facturation et veiller à ce que les opérations soient ajustées en fonction des besoins.  

Avant la mise en œuvre de l'ajustement des dates de facturation, la facture était basée sur la date anniversaire de facturation du partenaire, c'est-à-dire la date d'inscription du partenaire au programme Fournisseur de solutions Cloud, et non sur la date anniversaire de l'abonnement du client, c'est-à-dire la date d'achat de l'abonnement par le client. Après le 20février, les partenaires seront facturés à la date anniversaire de leur abonnement, ce qui élimine cette période de gratuité.  Les partenaires continueront de recevoir des factures à leur date anniversaire de facturation, mais la date d'effet de la facture correspondra à la date anniversaire d'abonnement du client. 

Les abonnements qui se trouvent dans la période gratuite au 20février ne seront pas facturés entre la date d'achat et la date de facturation du partenaire. En outre, le 1ermois de la période payante de 12mois ne sera pas facturé. Si vous utilisez un fichier de rapprochement pour vérification, n'oubliez pas que la facture de ce premier mois n'y sera plus visible.  


**Q:** Quelle est la nouveauté?

-   **R:** Les abonnements basés sur la licence ne bénéficieront plus de la période gratuite entre la date d'achat et la date de facturation du partenaire.

**Q:** Quand la période gratuite sera-t-elle supprimée?

- **R:** À compter du 20 février2018, les nouveaux abonnements n'auront pas de période gratuite.

**Q:** Les abonnements qui se trouvent dans la période gratuite au 20 février2018 seront-ils affectés?

- **R:** La période gratuite continuera jusqu'à la date de facturation du partenaire pour les abonnements qui se trouvent déjà dans la période gratuite au 20 février2018. En outre, le 1ermois de la période payante de 12mois ne sera pas facturé. Si vous utilisez le fichier de rapprochement pour vérification, n'oubliez pas que la facture de ce premier mois peut ne pas y figurer. Consultez les scénarios ci-dessous pour des explications plus détaillées.

**Q:** Quand commencera la période payante de 12mois?

- **R:** Actuellement, la période payante commence à la date de facturation du partenaire qui suit la date d'achat. Si la période gratuite est supprimée, la période payante des nouveaux abonnements commencera à la date d'achat.

**Q:** À quel moment les abonnements seront-ils automatiquement renouvelés?

- **R:** Actuellement, les abonnements sont automatiquement renouvelés 12mois après la date de facturation du partenaire qui suit la date d'achat. Si la période gratuite est supprimée, les abonnements seront automatiquement renouvelés 12mois après la date d'achat.

**Q:** Que se passe-t-il si j'achète l'abonnement le 29, le 30 ou le 31?

- **R:** L'abonnement sera fourni à la date d'achat, mais la période payante de 12mois ne démarrera pas avant le premier jour du mois suivant.

**Q:** Quelles sont les offres affectées par ce changement?

- **R:** Tous les abonnements basés sur la licence du programme Fournisseur de solution Cloud sont affectés.

**Q:** Comment ce changement affecte-t-il la facture et le fichier de rapprochement?

- **R:** Vous ne verrez plus la ligne «Facturation 0» qui représente la période de gratuité.

**Q:** Ma date de facturation changera-t-elle?

- **R:** Non, vous continuerez à recevoir la facture et le fichier de rapprochement à votre date de facturation existante.

**Q:** Les dates de début/fin de facturation mensuelle changeront-elles pour les abonnements existants?

- **R:** Non, les dates de début/fin de facturation mensuelle des abonnements existants continueront à correspondre à votre date de facturation. Toutefois, les nouveaux abonnements seront ajustés sur la date d'achat. Voir l'exemple ci-dessous.

**Q:** Le calcul des primes incitatives changera-t-il?

- **R:** Non

**Q:** Les API changeront-elles?

- **R:** Non

### <a name="common-scenarios"></a>Scénarios courants


|**Scénarios**   |**Scénario1: la période gratuite de l'abonnement se termine avant le 20février2018**   |**Scénario2: l'abonnement se trouve dans la période gratuite au 20février2018**  | **Scénario3: abonnement acheté à partir du 20 février2018**   |
|----------|:------------|:--------------------|:------------|
|Date d'achat |1erfévrier    | 1erfévrier    | 1er juin     |
|Date d'approvisionnement | 1erfévrier   |1erfévrier   |1erjuin   |
|Date de facturation   | 15   |25   | 15|
|Période gratuite   | 1erfévrier - 15février|1erfévrier - 24février   |Pas de période gratuite|
|Facture du 1ermois   | 15février - 14mars | 25février2018 - 24mars2018 Pas de facture, n'apparaît pas dans le fichier de rapprochement|1erjuin - 30juin   |
|Facture du 2emois   | 15mars - 14avril|25mars - 24avril   |1erjuillet - 31juillet|
|Début de la période payante   | 15février2018 | 25mars2018| 1erjuin2018| 
|Fin de la période payante | 14février2019   |24février2019   | 31mai2019  |
|Date de renouvellement | 15février2019 |25février2019   |1erjuin2019|

### <a name="scenario---new-purchase"></a>Scénario: nouvel achat

La date de facturation du partenaire est le 15. Le 1erjuin, le partenaire achète un nouvel abonnement à 30dollars/mois. Le fichier de rapprochement du 15juin contient les indications suivantes:

- Facture de 30dollars pour le 1ermois (1erjuin - 30juin)

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |

### <a name="scenario-suspend-and-reactivate-a-subscription-in-less-than-30-days-after-purchase"></a>Scénario: suspendre et réactiver un abonnement moins de 30jours après l'achat

La date de facturation du partenaire est le 15. Le 1erjuin, le partenaire achète un nouvel abonnement à 30dollars/mois. Le 5juin, le partenaire suspend l'abonnement. Le 10juin, le partenaire réactive l'abonnement. Le fichier de rapprochement du 15juin contient les indications suivantes:

- Facture de 30dollars pour le 1ermois (1erjuin - 30juin). 
- Crédit d'annulation de -30dollars. Notez que la date de début de facturation correspond au 5juin, date à laquelle le partenaire a suspendu l'abonnement. Le crédit n'est pas calculé au prorata. Le partenaire reçoit un crédit de 100% parce qu'il a suspendu l'abonnement au cours des 30premiers jours.
- Frais de réactivation de 30dollars. Notez que la date de début de facturation correspond au 10juin, date à laquelle le partenaire a réactivé l'abonnement. Le montant n'est pas calculé au prorata. Toutes les annulations et réactivations qui ont lieu dans les 30jours qui suivent la date d'achat ne font pas l'objet d'un calcul au prorata.


|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |
|05/06/2018   |30/06/2018   |-30dollars   |1   |30dollars   |
|10/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |


### <a name="scenario-suspend-a-subscription-in-less-than-30-days-after-purchase-and-reactivate-after-30-days"></a>Scénario: suspendre un abonnement moins de 30jours après l'achat et le réactiver après 30jours

La date de facturation du partenaire est le 15. Le 1erjuin, le partenaire achète un nouvel abonnement à 30dollars/mois. Le 5juin, le partenaire suspend l'abonnement. Le fichier de rapprochement du 15juin contient les indications suivantes:

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |
|05/06/2018   |30/06/2018   |-30dollars   |1   |30dollars   |

Le 10juillet, le partenaire réactive l'abonnement. Le fichier de rapprochement du 15juillet contient les frais suivants:

- Frais de réactivation de 21,29dollars. La date de début de facturation est le 10juillet, date à laquelle le partenaire a réactivé l'abonnement, et le montant est calculé au prorata à 21,29dollars. Toutes les annulations et réactivations qui ont lieu après les 30jours qui suivent la date d'achat font l'objet d'un calcul au prorata. 

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|10/07/2018   |31/07/2018   |21,29dollars   |1   |21,29dollars   |

La date de renouvellement de l'abonnement reste fixée au 1erjuin de l'année suivante, c'est-à-dire 12mois à compter de la date initiale d'achat.

### <a name="scenario-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Scénario: suspension et réactivation de l'abonnement plus de 30jours après l'achat 
La date de facturation du partenaire est le15 du mois. Le 1erjuin, le partenaire achète un nouvel abonnement d'une licence à 30dollars par mois. Le fichier de rapprochement du 15juin contient uniquement les indications suivantes: facture de 30dollars pour le 1ermois (1erjuin - 30juin).

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |

Le partenaire suspend l'abonnement le 5juillet mais le réactive le 15juillet. Le fichier de rapprochement du 15juillet contient les indications suivantes:

- Facture de 30dollars pour le 2emois (1erjuillet - 31juillet).

- Crédit d'annulation de -26,19dollars. Notez que la date de début de facturation est le 5juillet, date à laquelle le partenaire a suspendu l'abonnement, et que le crédit est calculé au prorata. Toutes les annulations et réactivations qui ont lieu après les 30jours qui suivent la date d'achat font l'objet d'un calcul au prorata.

- Frais de réactivation de 21,37dollars. Notez que la date de début de facturation est le 10juillet, date à laquelle le partenaire a réactivé l'abonnement, et que les frais sont calculés au prorata.

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/07/2018   |31/07/2018   |30dollars  |1   |30dollars   |
|05/07/2018   |31/07/2018   |   -26,19dollars   |1   |-26,19dollars|
|10/07/2018   |31/07/2018   |-21,37USD   |1   |21,37USD|

### <a name="scenario-change-license-quantity"></a>Scénario: modifier le nombre de licences 

La date de facturation du partenaire est le 15. Le 1erjuin, le partenaire achète un nouvel abonnement à 30dollars par mois. Le 10juin, le partenaire augmente la quantité de licences pour passer de1 à 2licences. Le fichier de rapprochement du 15juin contient les indications suivantes:

- Facture de 30dollars pour le 1ermois (1erjuin - 30juin). Même si le partenaire a augmenté le nombre de licences avant la date de facturation du 15juin, cette modification ne sera pas prise en compte dans le système de facturation Microsoft jusqu'au jour anniversaire de l'abonnement le 1erjuillet.

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |

Le 1erjuillet, le jour anniversaire de l'abonnement, le système de facturation Microsoft prend en compte le fait que le nombre de licences a été modifié pour passer de1 à2 le 10juin. Le système de facturation génère un crédit et une facture calculés au prorata pour le 1ermois et une facture pour le 2emois. Le fichier de rapprochement du 15juillet contient les indications suivantes:

- Crédit de -30dollars pour le 1ermois.
- Frais de 9dollars calculés au prorata pour le 1ermois (1erjuin - 9juin) pour 1licence.
- Frais de 42dollars calculés au prorata pour le 1ermois (10juin - 30juin) pour 2licences.
- Facture de 60dollars pour le 2emois (1erjuillet - 31juillet) pour 2licences.

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |-30dollars   |1   |-30dollars|
|01/06/2018   |09/06/2018   |9dollars   |1   |9dollars|
|10/06/2018   |30/06/2018   |21dollars   |2   |42dollars|
|01/07/2018   |31/07/2018   |30dollars   |2   |60dollars   |

### <a name="scenario-add-on-subscriptions"></a>Scénario: abonnements à des modules complémentaires

La date de facturation du partenaire est le 15. Le 1erjuin, le partenaire achète un nouvel abonnement à 30dollars par mois. Le 10juin, le partenaire achète un nouvel abonnement au module complémentaire à 5dollars par mois. La date de renouvellement de l'abonnement au module complémentaire sera ajusté sur la date de renouvellement de l'abonnement de base qui est le 1erjuin. 

Le fichier de rapprochement du 15juin contient les indications suivantes:

- Facture de 30dollars pour le 1ermois (1erjuin - 30juin). Cela concerne l'abonnement de base.
- Frais de 3,50dollars calculés au prorata pour le 1ermois (10juin - 30juin) pour l'abonnement au module complémentaire. La date de début de facturation est le 10juin, date à laquelle le partenaire a acheté l'abonnement au module complémentaire, et le montant est calculé au prorata.

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   |30/06/2018   |30dollars   |1   |30dollars   |
|10/06/2018   |30/06/2018   |3,50USD   |1   |3,50USD   |

Le fichier de rapprochement du 15juillet contient les indications suivantes:

- Facture de 30dollars pour le 2emois (1erjuillet - 31juillet). Cela concerne l'abonnement de base.
- Facture de 5dollars pour le 2emois (1erjuillet - 31juillet). Cela concerne l'abonnement au module complémentaire.

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/07/2018   |31/07/2018   |30dollars   |1   |30dollars   |
|01/07/2018   |31/07/2018   |5dollars   |1   |5dollars   |

### <a name="scenario-new-purchase-on-the-29th-30th-or-31st"></a>Scénario: nouvel achat le 29, le 30 ou le 31 

La date de facturation du partenaire est le15 du mois. Le 29mai, le partenaire achète un nouvel abonnement (1licence à 30USD/mois) avec une fréquence de facturation mensuelle. La date anniversaire pour les abonnements achetés le 29, 30 ou 31 est par défaut le 1er. Dans ce scénario, l'abonnement sera gratuit du 29mai au 31mai, et la ligne de facturation apparaîtra le 1erjuin affichant l'avance de frais pour un mois.

Le fichier de rapprochement du 15juin contient les indications suivantes:

- Facture de 30dollars pour le 1ermois (1erjuin - 30juin)

|**Début de facturation**   |**Fin de facturation**   |**Prix unitaire**   |**Quantité**   |**Montant**   |
|-----------------|:-------------|:----------------|:------------|:------|
|01/06/2018   | 30/06/2018   |30dollars   |1   |30dollars  |
