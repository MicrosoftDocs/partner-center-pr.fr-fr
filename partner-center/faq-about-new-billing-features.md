---
title: FAQ sur les nouvelles fonctionnalités de facturation | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
Description: Vous trouverez ci-dessous les réponses aux questions fréquemment posées à propos de la facturation annuelle et des essais gratuits de l’Espace partenaires.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: d595c05adac5ffc57a52d8635abf80cb0b3f375d
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820311"
---
# <a name="faq-about-new-billing-features"></a>FAQ sur les nouvelles fonctionnalités de facturation

**S’applique à**

-  Espace partenaires
-  Espace partenaires de Microsoft Cloud for US Government


Vous trouverez ci-dessous les réponses aux questions fréquemment posées à propos de la facturation annuelle et des essais gratuits de l’Espace partenaires. 

## <a name="in-this-section"></a>Dans cette section

-   [FAQ sur la facturation annuelle](#annualbillingfaq)

-   [FAQ sur les essais gratuits](#freetrialsfaq)

-   [FAQ sur l’alignement de la facturation](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>FAQ sur la facturation annuelle

Sections :

[Vue d’ensemble et avantages de la facturation annuelle](#overviewandbenefits)

[Placement de vos scénarios de commande et de facturation](#placingyourorder)

[Modification de votre abonnement](#changingyoursubscription)

[Calcul de la tarification](#pricingcalculation)

[Comptes](#reporting)

[Visant](#incentives)


<a href="" id="overviewandbenefits"></a>**Vue d’ensemble et avantages de la facturation annuelle**

**Q :** Qu’est-ce qui a changé?

-   **R :** En réponse à vos demandes, nous avons introduit l’option de paiement de certains abonnements CSP sur une base annuelle ou mensuelle. Cette nouvelle option sera disponible le 17 octobre 2017.

**Q :** Qui peut participer?

-   **R :** Tous les partenaires et types de partenaires peuvent bénéficier de la facturation annuelle. La facturation annuelle est disponible dans tous les marchés où le programme Fournisseur de solutions Cloud est actuellement disponible. 

**Q :** Que dois-je prendre en considération pour réfléchir à la facturation annuelle?    

-   **R :** Vous devez réfléchir à la façon dont votre mouvement de vente sera affecté. Voici quelques conseils pour vous aider à utiliser efficacement la facturation annuelle. 
    - Mettez à jour les API pour prendre en compte la fonctionnalité de facturation annuelle, le cas échéant. 
    - Examinez les modifications apportées à la facture et au fichier de rapprochement basé sur les licences.
    - Assurez-vous que votre équipe est informée.
    - Mettez à jour vos processus internes si nécessaire.

**Q :** Quels sont les avantages de la facturation annuelle? 

-   **R :** La facturation annuelle offre les avantages suivants:

    - Flexibilité accrue en matière d'options de paiement.

    - Meilleur alignement avec la facturation de vos clients.

    - Réduction de l'impact des fluctuations de devises.

    - Réduction des coûts d’exploitation en matière de facturation.

**Q :** Quelles offres peuvent être facturées annuellement?

-   **R :** La plupart des abonnements basés sur une licence ont la possibilité d’utiliser l’option de facturation mensuelle ou annuelle. Les abonnements basés sur l’utilisation proposent uniquement une facturation mensuelle. Vous pouvez consulter les fréquences de facturation disponibles pour chaque offre dans la colonne J du tableau des offres. Vous trouverez le tableau des offres dans la section « Voir les offres et leur tarification » de l'Espace partenaires. .

**Q :** La facturation annuelle est-elle par abonnement ou par licence?       

-   **R :** La facturation annuelle et mensuelle sont par abonnement.

**Q :** Y a-t-il des modifications nécessaires aux API pour prendre en charge la facturation annuelle?    

-   **R :** Pour tirer parti de la facturation annuelle, vous devez modifier vos API. Vous trouverez plus d’informations dans les articles suivants :

    - https://partnercenter.microsoft.com/partner/developer

    - https://msdn.microsoft.com/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Exemple de code : https://msdn.microsoft.com/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Placement de vos scénarios de commande et de facturation**

**Q :** Existe-t-il une offre unique spécifique pour les commandes avec facturation annuelle?   

-   **R :** Non. Toutes les fréquences de facturation, y compris l'option de facturation annuelle, sont affectées à l’offre sous forme d'attribut. Toutefois, vous pouvez donner à une offre un nom plus explicite pour aider les clients à faire facilement la distinction.

**Q :** Comment faire sélectionnez la facturation annuelle?

-   **R :** Lorsque vous ajoutez un nouvel abonnement, vous êtes invité à choisir la fréquence de facturation. Vous pouvez choisir l’option de facturation annuelle à ce stade. Une fois la facturation annuelle sélectionnée, toutes les offres disponibles s'affichent.

**Q :** Si je choisis la facturation annuelle quand est-ce que je suis facturé?    

-   **R :** Vous serez facturé à la prochaine date de facturation. Par exemple, si votre date de facturation est fixée au 1er du mois, et que vous achetez un abonnement facturé à l'année le 29 octobre 2017, vous serez facturé le 1er novembre 2017. Si vous n’apportez aucune modification à la licence, vous serez facturé à nouveau le 1er novembre 2018. Si vous modifiez une licence, vous serez crédité et refacturé à la date de facturation suivante. 

**Q :** Puis-je fractionner un abonnement de sorte qu’une partie soit facturée mensuellement et que l’autre soit facturée annuellement?  

-   **R :** Non. L’intégralité de l’abonnement doit avoir la même fréquence de facturation. L’intégralité de l’abonnement doit donner lieu à une facturation mensuelle ou annuelle.

**Q :** Quand le renouvellement de l’abonnement à Al est-il associé à la facturation annuelle?     

-   **R :** La date de renouvellement sera de douze mois après la date de début du service. La période de service commence à la date de création de l’abonnement.  Par exemple, un abonnement créé le 10 janvier 2018 sera renouvelé le 10 janvier 2019.

**Q :** Quand suis-je facturé pour le renouvellement d’un abonnement avec une facturation annuelle? 

-   **R :** Vous serez facturé à la prochaine date de facturation suivant la date de renouvellement de l’abonnement. Par exemple, si vous achetez un abonnement à facturation annuelle le 15 janvier 2018 et que votre date de facturation est le 20 janvier, votre abonnement sera renouvelé le 15 janvier 2019. Vous serez facturé pour le renouvellement le 20 janvier 2019.

**Q :** Les abonnements avec facturation annuelle reçoivent-ils une période gratuite?

-   **R :** Non, les abonnements avec une fréquence de facturation annuelle ne bénéficient pas d’une période gratuite. La période d'abonnement de 12 mois commence à la date d’achat. Ces conditions diffèrent de celles des abonnements à fréquence de facturation mensuelle qui bénéficient d'une période gratuite entre la date d’achat et la date de facturation qui suit.

**Q :** Un client peut-il avoir plusieurs abonnements de la même offre, chacun avec des fréquences de facturation différentes?    

-   **R :** Cela dépend de l’offre. Certaines offres sont limitées à un abonnement par client. Si l’offre n’est pas limitée, un client peut avoir plusieurs abonnements d'une même offre avec des fréquences de facturation différentes. Vous trouverez les détails des limites et restrictions de chaque offre dans la colonne I du tableau des offres. Vous trouverez le tableau des offres dans la section « Voir les offres et leur tarification » de l'Espace partenaires.

<a href="" id="changingyoursubscription"></a>**Modification de votre abonnement**

**Q :** Puis-je ajouter une nouvelle licence à un abonnement existant qui a une facturation annuelle?    

-   **R :** Oui. Vous pouvez modifier le nombre de licences de vos abonnements à tout moment. L'ajout de licences supplémentaires n’aura aucune incidence sur la fréquence de facturation. 

**Q :** Puis-je ajouter des licences qui ont une facturation mensuelle à un abonnement existant qui a une facturation annuelle? 

-   **R :** Une fois que vous avez acheté un abonnement avec la facturation annuelle, toutes les licences supplémentaires suivent la même fréquence de facturation. Si par la suite vous devez acheter des licences à facturation mensuelle, vous devrez acheter un nouvel abonnement.

**Q :** Puis-je basculer la fréquence de facturation d’un abonnement de mensuelle à annuelle et vice versa? 

-   **R :** Oui. **Pour modifier la fréquence de facturation d’un service en ligne** , consultez la page de base sur la [facturation](https://docs.microsoft.com/partner-center/billing-basics).

**Q :** La facturation annuelle est-elle disponible pour les offres complémentaires?   

-   **R :** Oui. L'abonnement au module complémentaire aura automatiquement la même fréquence de facturation que l’abonnement parent.

**Q :** Comment le travail de facturation annuel sera-t-il possible lorsque j’ajoute ou supprime des licences? 

-   **R :** Vous pouvez ajouter ou supprimer des licences à tout moment. Vous recevrez un crédit et une refacturation au prorata lors de la prochaine date de facturation qui suit la modification du nombre de licences. 

**Q :** Que se passe-t-il si j’annule un abonnement avec un travail de facturation annuelle?    

-   **R :** La stratégie d’annulation est la même pour toutes les fréquences de facturation. Si l'abonnement est supprimé dans les 30 premiers jours de la période payante de 12 mois, vous recevrez un crédit de 100 % à la date de facturation suivante. Si l’abonnement est annulé 30 jours après le début de la période d'abonnement de 12 mois, vous serez crédité au prorata à la date de facturation suivante.

**Q :** Un client peut-il déplacer un abonnement avec une facturation annuelle d’un partenaire à un autre?  

-   **R :** Non. Les abonnements ne peuvent pas être transférés entre des partenaires. Le nouveau partenaire doit acheter un nouvel abonnement pour le compte du client. Cela s’applique aussi bien aux abonnements à facturation mensuelle qu'annuelle.

**Q :** Puis-je réactiver un abonnement avec la facturation annuelle?

-   **R :** Oui, vous pouvez réactiver l’abonnement pendant jusqu’à 90 jours à partir de la date de la suspension. Les frais calculés au prorata seront facturés à la date de facturation suivante. La date de renouvellement de l’abonnement reste identique.

<a href="" id="pricingcalculation"></a>**Calcul de la tarification**

**Q :** Que se passe-t-il si le prix d’une offre est modifié dans le cadre de la période de 12 mois d’un abonnement facturé annuellement?    

-   **R :** Le tarif de l’offre au moment de l’achat est garanti pour la durée d’abonnement complète de 12 mois. 

**Q :** Sur quel prix un abonnement sera-t-il effectué après une période d’abonnement de 12 mois?    

-   **R :** Lorsqu’un abonnement renouvelle, le prix est basé sur la liste de prix actuelle à la date du renouvellement. Le nouveau prix est garanti pour la période des 12 mois suivants de l’abonnement.

**Q :** Comment le crédit d’une licence ou d’un abonnement annulé (e) est-il calculé? Est-il calculé à la journée ou au mois ?   

-   **R :** Le crédit d’annulation est calculé comme suit:

    - Crédit d’annulation = ((prix mensuel*12)/365) * nombre de jours restants dans la période de 12 mois * nombre de licences annulées.

**Q :** Que se passe-t-il si le prix d’une offre diminue d’une partie de la période de 12 mois d’un abonnement facturé annuellement? 

-   **R :** Aucune modification n’est apportée. Le prix est défini pour toute la période de 12 mois. Il en va de même pour une facturation mensuelle.


<a href="" id="reporting"></a>**Comptes**

**Q :** Où puis-je savoir si un abonnement est facturé annuellement ou mensuellement?   

-   **R :** Le fichier de réconciliation basé sur les licences inclut les informations sur la fréquence de facturation. Vous les trouverez dans la colonne AA

**Q :** Quelles sont les modifications que je vois dans le fichier de réconciliation basé sur les licences lorsque l’abonnement avec facturation annuelle est acheté ou renouvelé?  

-   **R :** La première modification sera une nouvelle ligne dans le fichier de rapprochement basé sur licence à la première date de facturation suivant l’achat ou un nouvel abonnement. . Si aucune modification n'est apportée à l’abonnement, aucune ligne n'apparaît sur les fichiers de rapprochement pour les mois 2 à 12 de la période d'abonnement. La prochaine modification apportée au fichier de rapprochement s’affiche lors du renouvellement de l’abonnement. Elle s’affiche à la première date de facturation qui suit le renouvellement. Si une modification est apportée à l’abonnement au cours de la période de 12 mois, un crédit et une refacturation au prorata apparaîtront sur le prochain fichier de rapprochement qui suit la modification.

**Q :** Comment l’achat de, le changement ou l’annulation d’un abonnement annuel apparaissent-ils dans la colonne P des fichiers d’utilisation?

-   **R :** Les frais d’achat initiaux s’affichent sous la forme «frais de prorata lors de l’achat». Les modifications de licence qui font l'objet d'un crédit et d'une refacturation s’affichent sous forme d'« Instance de cycle au prorata ». Les crédits d’annulation apparaissent sous forme de « Frais d'annulation ».

**Q :** Lorsqu’un abonnement annuel est annulé, comment cela apparaît-il sur le fichier de réconciliation?   

-   **R :** Le fichier de réconciliation contient un élément de ligne pour un crédit d’annulation. Si l’annulation se produit dans les 30 premiers jours de la période de 12 mois, l’abonnement sera crédité à 100 %. Si l’annulation se produit après les 30 premiers jours, l’abonnement sera crédité au prorata.

**Q :** Comment s’affiche-t-il dans le fichier de rapprochement si des licences sont ajoutées à un abonnement qui a une facturation annuelle?  

-   **R :** Le fichier de réconciliation contient un crédit et une facture au prorata. C'est également le cas pour un abonnement à facturation mensuelle.

**Q :** Comment apparaît-t-il le fichier de rapprochement si les licences sont supprimées d’un abonnement avec facturation annuelle? 

-   **R :** Le fichier de réconciliation contient un crédit et une facture au prorata.  C'est également le cas pour un abonnement à facturation mensuelle.

**Q :** Le prix annuel est-il indiqué sur la liste de prix? 

-   **R :** Non. La liste de prix indique le prix mensuel. Vous pouvez calculer le prix annuel en multipliant le prix mensuel par douze.

**Q :** La matrice d’offre a-t-elle des entrées différentes pour les offres qui peuvent être facturées annuellement?   

-   **R :**  Non. Les identifiants des offres sont les mêmes pour toutes les fréquences de facturation. Il n'existe pas d'identifiant unique pour les offres à facturation annuelle.


<a href="" id="incentives"></a>**Visant**

**Q :** À quelle fréquence les incentives sont-ils calculés sur des abonnements annuels? 

-   **R :** Nous calculons le chiffre d’affaires facturé. Les paiements des primes obtenues seront versés conformément à notre stratégie présentée dans nos guides des primes du programme Fournisseur de solutions Cloud. 

**Q :** Comment les incentives sur les abonnements facturés annuel sont-ils payés?  

-   **R :** Actuellement, tous les paiements d’incentives sont effectués deux fois par an. Ces paiements sont versés 45 jours après la fin du semestre.

**Q :** Lorsqu’un abonnement facturé annuellement est vendu, comment les revenus de cet abonnement seront-ils reconnus pour le calcul des incentives. Le calcul est-il basé sur les revenus payés ou ajustés ? 

-   **R :** Les calculs d’incentives sont basés sur le chiffre d’affaires facturé.

**Q :** Comment les bénéfices des primes incitatives sur les abonnements à facturation annuelle éligibles sont-ils calculés parmi les différents taux de primes du programme Fournisseur de solutions Cloud (taux de primes mondiaux, taux accélérateurs locaux et campagnes locales) ?

-   **R :** Quelle que soit la façon dont un abonnement est facturé, mensuel ou annuellement, les partenaires peuvent gagner des incentives sur toutes les transactions éligibles. Cela inclut le taux de prime mondial, appliqué au revenu facturé pour la période, l’accélérateur local pour toutes les régions où il existe des accélérateurs locaux et les campagnes mondiales, le cas échéant.

**Q :** Qui peut vous contacter si vous avez des questions sur les incentives?

- **R :** Veuillez contacter l’équipe de support technique régional appropriée:

  - Amérique du Nord : ocina@microsoft.com

  - Amérique latine et Brésil : ocilatam@microsoft.com

  - EMEA : ociemea@microsoft.com

  - APOAC (à l'exception du Japon) : ociapgc@microsoft.com

  - Japon : ocijp@microsoft.com


**Q :** Que se passe-t-il si je suspend mon abonnement? 

-   **R :** Si vous suspendez un abonnement, que ce soit dans l’espace partenaires ou via l’API, dans les 30 jours suivant votre achat, vous recevrez un crédit de 100%, quelle que soit la fréquence de facturation. 

    Avec une facturation annuelle, cela se présenterait comme suit :

    - Achat par le partenaire d'un abonnement le 1er janvier = création d'une ligne de facturation de frais pour la période de service du 01/01 au 31/12.
    - Suspension de l'abonnement le 25 janvier = création d'une ligne de facturation de crédit pour la période de service du 01/01 au 31/12.
    - Réactivation le 29 janvier = création d'une ligne de facturation de frais pour la période de service du 29/01 au 31/12.

    Avec une facturation mensuelle, cela se présenterait comme suit :

    - Achat par le partenaire d'un abonnement le 1er janvier = création d'une ligne de facturation de frais pour la période de service du 01/01 au 31/12.
    - Suspension de l'abonnement le 25 janvier = création d'une ligne de facturation de crédit pour la période de service du 01/01 au 31/01.
    - Réactivation le 29 janvier = création d'une ligne de facturation de frais pour la période de service du 29/01 au 31/01.



## <a href="" id="freetrialsfaq"></a>FAQ sur les essais gratuits

**1ER** Que sont les versions d’évaluation gratuites?

-   **R :** Vous pouvez proposer à vos clients une version d’évaluation gratuite de 30 jours de certains produits. Cela leur permet d’évaluer le produit avant de l’acheter. Des essais gratuits sont proposés pour les produits suivants : 

    - Office 365 Business Premium (depuis le 17 octobre 2017)
    - Office 365 E3 (depuis le 17 octobre 2017)
    - Office 365 E5 avec PSTN (depuis le 17 octobre 2017)
    - Office 365 E5 sans PSTN (depuis le 17 octobre 2017)
    - Enterprise Mobility + Security E5 (depuis le 17 octobre 2017)
    - Formule Dynamics 365 Customer Engagement 1 (depuis le 17 octobre 2017)
    - Dynamics 365 for Financials (depuis le 17 octobre 2017)
    - Microsoft 365 Business (au 1er mars 2018)
    
**Q2** La facturation annuelle et les versions d’évaluation gratuites diffèrent-elles dans le cloud Souverain et le cloud public?

-   **R :** Non. Ils sont identiques. La seule différence réside dans les références d’évaluation qui sont disponibles au moment du lancement.

**Q3** Qui peut participer?

-   **R :** Tous les partenaires peuvent participer. Toutefois, ce programme n’est actuellement pas disponible en Chine. 

**4ÈME** Quelles actions dois-je entreprendre pour me permettre de bénéficier de ces versions d’évaluation gratuites?

-   **R :** Réfléchissez à la façon dont l’essai gratuit peut être intégré à votre mouvement de vente et à l’impact sur vos processus internes. Vous devrez peut-être également modifier vos API pour prendre en charge la conversion d’un essai gratuit en abonnement payant. Des spécifications techniques détaillées pour les modifications apportées aux API sont présentées dans la vue Annonces de l'Espace partenaires.

**Q5** L’essai gratuit s’affiche-t-il sur mon fichier de facture et de rapprochement?

-   **R :** Non, les versions d’évaluation gratuites n’apparaissent pas sur votre facture ou fichier de réconciliation basé sur une licence. Ils apparaîtront dans votre facture et votre fichier de rapprochement basé sur la licence une fois que vous les aurez convertis en abonnements payants. Un abonnement converti s’affiche à la fois sur votre facture et sur votre fichier de rapprochement basé sur la licence, de la même manière qu'un nouvel abonnement.

**Q6** Les essais gratuits ont-ils un impact sur les incentives?

-   **R :** Non. L’essai gratuit n’aura aucun impact sur les primes.

**Q7** Les versions d’évaluation seront-elles disponibles pour d’autres produits Office à l’avenir?

-   **R :** Nous fournissons des essais gratuits pour ces produits, parce qu'il s'agit des offres commerciales les plus complètes et les plus populaires. Il se peut que nous ajoutions d'autres offres d'essais gratuits à l’avenir.

**Q8** Un client peut-il avoir plusieurs essais gratuits?

-   **R :** Chaque client bénéficie d’un essai gratuit par offre disponible.

**Q9** Existe-t-il des limites pour une version d’évaluation gratuite?

-   **R :** Oui. L'essai est valable pour un maximum de 25 licences. Le nombre de licences ne peut pas être modifié pendant la période d'essai. Une fois l’essai converti en abonnement payant, vous pouvez lui ajouter des licences supplémentaires.

**Q10** Une version d’évaluation gratuite est-elle automatiquement convertie en abonnement payant?

-   **R :** Non. Vous devez convertir l’abonnement vous-même, dans l'Espace partenaires ou via l’API.

**Q11** Les versions d’évaluation peuvent-elles être utilisées à la fois pour les abonnements mensuels et annuels?

-   **R :** Oui. Vous choisissez la fréquence de facturation lorsque vous convertissez l'essai en abonnement payant.

**Q12** La date de début de l’abonnement sera-t-elle basée sur la date de début de la version d’évaluation gratuite ou la date à laquelle elle est convertie en abonnement payant? 

-   **R :** La date de début est basée sur la date de conversion. Si l'essai gratuit est converti en offre payante à facturation annuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de conversion. Si l'essai gratuit est converti en une offre payante avec facturation mensuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de facturation suivant la date de conversion.

**Q13:** Puis-je ajouter ou supprimer des sièges pendant la période d’évaluation gratuite?

-   **R :** Non. Le nombre de licences par défaut pour les essais gratuits sera égal à 25 et ne pourra pas être modifié.

**Q14:** Existe-t-il des versions d’évaluation pour les offres d’ajout comme ATP et RTPC?

-   **R :** Il n’y a pas d’essai gratuit pour les offres complémentaires pour l’instant.

**Q15:** Puis-je fournir une version d’évaluation gratuite pour une offre déjà détenue par un client?

-   **R :** Non. Si le client possède déjà l’offre, elle ne peut pas être utilisée pour un essai gratuit.

**Q16:** Suis-je en mesure de voir toutes les offres d’essai en suspens?

-   **R :** Oui. La page du client répertorie tous les abonnements. Elle indique à la fois les abonnements d’essai gratuit et les abonnements payants.

**Q17:** Suis-je averti de l’expiration des essais gratuits?

-   **R :** Non. Vous pouvez suivre les dates d’expiration à venir soit à l’aide de la vue des clients dans l’Espace partenaires, soit en interrogeant l’API. Il est recommandé de contrôler fréquemment ces dates afin de pouvoir prendre les mesures de suivi appropriées auprès des clients à l’approche du moment où ils doivent prendre une décision.

**Q18:** Si un client dispose d’un essai gratuit pour une offre, peut-il utiliser également une autre version d’évaluation pour une autre offre? 

-   **R :** Oui. Les clients peuvent souscrire un essai par offre. Par exemple, ils peuvent obtenir un essai gratuit pour Office 365 Business Premium et un autre pour Office 365 E3.

**Q19:** Que se passe-t-il quand la version d’évaluation se termine? Mon client ou moi allons-nous recevoir une notification ? Quelles notifications apparaissent-elles lors d'une tentative de connexion à un essai arrivé à expiration ?

-   **R :** Une fois qu’un essai a expiré, un client qui tente de se connecter à cette version d’évaluation voit un message indiquant que l’essai a expiré. Aucune notification ne sera envoyée pour indiquer qu’un essai arrive à expiration, mais en tant que partenaire, vous pouvez en assurer le suivi en consultant la vue des clients ou par l’intermédiaire de requêtes à l’API.

**Q20:** Une version d’évaluation peut-elle être étendue?

-   **R :** Non. Au bout de 30 jours, l'essai doit être converti, sinon, il expirera.

**Q21:** Quand une version d’évaluation arrive à expiration, puis-je accéder aux informations de la version d’évaluation?

-   **R :** Oui. Les données sont stockées conformément aux normes de conservation des données. Dès que vous achetez un nouvel abonnement avec les mêmes plans de service, les données de vos clients sont accessibles à partir de l’abonnement qui vient d’être activé.

**Q22:** Des versions d’évaluation gratuites sont-elles disponibles pour les offres gouvernementales et de formation?

-   **R :** Il n’y a pas d’essai gratuit pour les offres gouvernementales et de formation pour le moment.

**Q23:** Les versions d’évaluation gratuites du programme du fournisseur de solutions Cloud (CSP) peuvent-elles être converties en d’autres locataires de programme tels que EA, Open ou MOSP? 

-   **R :** Non. Les abonnements ne peuvent pas être transférés du programme fournisseur de solutions Cloud vers un autre programme.

**Q24:** Comment puis-je bénéficier d’un support technique sur les versions d’évaluation gratuites? 

-   **R :** Envoyez une demande de service via l’espace partenaires.

## <a href="" id="billingalignmentfaq"></a>Alignement de la facturation-fin de la période libre

Dès le 21 février 2018, le programme de fournisseur de solutions Cloud débutera la mise en œuvre de « l'ajustement des dates de facturation » pour les nouveaux abonnements à fréquence de facturation mensuelle. Cet « ajustement des dates de facturation » donnera une plus grande flexibilité aux partenaires ainsi qu'une meilleure prévision de leurs ventes et de leur facturation. Il permettra en outre un meilleure approvisionnement et une meilleure gestion des abonnements des clients. 

**MISE à jour du 23 février:**  Nous avions précédemment annoncé la date de mise en œuvre du 20 février, mais en réalité, notre implémentation a été légèrement différée et répartie par catégorie de produit.  Veuillez passer en revue le tableau ci-dessous pour connaître la date de mise en œuvre par catégorie de produit. 

|**Catégorie de produit**   |**Jour de la mise en œuvre**   |
|-----------------|:-------------|
|Office  |21 février   |
|Windows, Minecraft   |22 février   |
|Office 365 Chine   |23 février   |
|Dynamics/Intune   |23 février   |

Les abonnements achetés avant la date de mise en œuvre (voir le tableau ci-dessus) bénéficient d'une période gratuite entre la date d’achat et la date de facturation du partenaire. Les abonnements achetés après la date de mise en œuvre ne bénéficieront plus de la période de gratuité. La période payant de douze mois démarrera (s'ajustera) à la date d'achat en fonction de la facturation du partenaire. Les partenaires ne verront plus la ligne « Facturation 0 » qui représente la période de gratuité sur le fichier de rapprochement. Aucune modification n’est apportée aux API de facturation ou aux primes incitatives.  Les partenaires doivent informer leurs équipes de vente et de gestion des comptes de cette nouvelle logique de facturation et veiller à ce que les opérations soient ajustées en fonction des besoins.  

Avant la mise en œuvre de l’ajustement des dates de facturation, la facture était basée sur la date anniversaire de facturation du partenaire, c'est-à-dire la date d'inscription du partenaire au programme Fournisseur de solutions Cloud, et non sur la date anniversaire de l'abonnement du client, c'est-à-dire la date d'achat de l'abonnement par le client. Après la date de mise en œuvre, les partenaires seront facturés à la date anniversaire de leur abonnement, ce qui élimine cette période de gratuité.  Les partenaires continueront de recevoir des factures à leur date anniversaire de facturation, mais la date d’effet de la facture correspondra à la date anniversaire d’abonnement du client. 

Les abonnements qui se trouvent dans la période gratuite à la date de mise en œuvre ne seront pas facturés entre la date d’achat et la date de facturation du partenaire. En outre, le 1er mois de la période payante de 12 mois ne sera pas facturé. Si vous utilisez un fichier de rapprochement pour vérification, n'oubliez pas que la facture de ce premier mois n'y sera plus visible.  

**1ER** Qu’est-ce qui change avec la date de facturation?

-   **R :** Les abonnements basés sur une licence ne disposent plus d’une période libre. Actuellement, il existe une période gratuite entre la date d'achat et la date de facturation du partenaire.

**Q2** Quand la période libre sera-t-elle supprimée?

- **R :** À partir de la date de mise en œuvre indiquée dans le tableau ci-dessous, les nouveaux abonnements ne recevront pas de période gratuite.

|**Catégorie de produit**   |**Jour de la mise en œuvre**   |
|-----------------|:-------------|
|Office  |21 février   |
|Windows, Minecraft   |22 février   |
|Office 365 Chine   |23 février   |
|Dynamics/Intune   |23 février   |

**Q3** Quel sera l’impact sur les abonnements pendant la période libre à la date d’implémentation?

- **R :** Les abonnements qui se trouvent dans la période libre à la date de mise en œuvre recevront toujours une période gratuite allant de la date d’achat à la date de facturation du partenaire. Ces licences bénéficient également d'une « période gratuite étendue » et le 1er mois de la période payante de 12 mois ne sera pas facturé. La « période gratuite étendue » ne s'appliquera pas aux licences ajoutées lors du 1er mois. Si vous augmentez la quantité de licences lors du 1er mois, vous serez facturé pour les licences ajoutées sur la facture/le rapprochement suivant. Si vous utilisez le fichier de rapprochement pour vérification, n’oubliez pas que la facture de ce premier mois peut ne pas y figurer. Consultez les scénarios ci-dessous pour des explications plus détaillées.

**4ÈME** Quand la période de 12 mois payante commence-t-elle pour un nouvel abonnement?

- **R :** Actuellement, la période payée commence à la date de facturation du partenaire qui suit la date d’achat. À partir de la date de mise en œuvre, la période payante des nouveaux abonnements commencera à la date d’achat.

**Q5** Quand les abonnements seront-ils renouvelés automatiquement?

- **R :** Les abonnements sont renouvelés automatiquement 12 mois après la première date de facturation. Actuellement, cela signifie que les abonnements sont automatiquement renouvelés 12 mois après la première date de facturation du partenaire qui suit la date d’achat. À compter de la date de mise en œuvre, les nouveaux abonnements seront renouvelés automatiquement 12 mois après la date d’achat.

**Q6** Que se passe-t-il si j’achète l’abonnement le 29, le 30 ou le 31 du mois?

- **R :** L’abonnement sera disponible à partir de la date d’achat, mais le délai payé de 12 mois ne commencera pas avant le premier jour du mois suivant.

**Q7** Quelles sont les offres affectées?

- **R :** La suppression de la période gratuite s’applique à tous les abonnements basés sur des licences CSP.

**Q8** Comment cela affecte-t-il la facture et le fichier de rapprochement? 

- **R :** Vous ne verrez plus la «ligne de facturation $0» sur la facture ou le fichier de réconciliation. Actuellement, la ligne « Facturation 0 » représente la période gratuite.

**Q9** La date de facturation change-t-elle?

- **R :** Non, vous continuerez à recevoir la facture et le fichier de rapprochement à la date de facturation existante.

**Q10** Les dates de début et de fin des frais mensuelles seront-elles modifiées pour les abonnements existants?

- **R :** Non, les dates de début et de fin des frais mensuels d’abonnement existants continuent de s’aligner sur la date de facturation. Toutefois, les nouveaux abonnements seront ajustés sur la date d’achat. Voir l'exemple ci-dessous.

**Q11** Le calcul des incentives sera-t-il modifié?

- **R :** Non, aucune modification n’est apportée aux calculs d’incentives.

**Q12** Y aura-t-il une modification des API?

- **R :** Non, aucune modification n’est apportée aux API.

### <a name="common-scenarios"></a>Scénarios courants


|**Scénarios**   |**Scénario 1 : La période libre d’abonnement se termine avant la date de mise en œuvre**   |**Scénario 2 : L’abonnement est dans la période libre à la date de mise en œuvre**  | **Scénario 3: Abonnement acheté le ou après la date de mise en œuvre**   |
|----------|:------------|:--------------------|:------------|
|Date d’achat |1er février 2018    | 1er février 2018    | 1er juin 2018     |
|Date d'approvisionnement | 1er février 2018   |1er février 2018   |1er juin 2018   |
|Date de facturation   | 15 du mois   |25 du mois   | 15 du mois|
|Période gratuite   | Du 1er février 2018 au 14 février 2018|Du 1er février 2018 au 24 février 2018   |Pas de période gratuite|
|Facture du 1er mois   | Du 15 février 2018 au 14 mars 2018 | La quantité de licences au 24 février 2018 recevra une période gratuite étendue jusqu'au 24 mars 2018. Les licences ajoutées après le 24 février 2018 seront facturées. |Du 1er juin 2018 au 30 juin 2018   |
|Facture du 2e mois   | Du 15 mars 2018 au 14 avril 2018|Du 25 mars 2018 au 24 avril 2018   |Du 1er juillet 2018 au 31 juillet 2018|
|Début de la période payante   | 15 février 2018 | 25 février 2018| 1er juin 2018| 
|Fin de la période payante | 14 février 2019   |24 février 2019   | 31 mai 2019  |
|Date de renouvellement | 15 février 2019 |25 février 2019   |1er juin 2019|

### <a name="scenario-4---new-purchase"></a>Scénario 4 : nouvel achat

La date de facturation du partenaire est le 15e jour du mois. Le 1er juin 2018, le partenaire achète un nouvel abonnement. Le prix de l’abonnement est défini à 30 $ par licence par mois. 

Le fichier de rapprochement du 15 juin contiendra uniquement les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Scénario 5A: Interrompre et réactiver avant la date de facturation

La date de facturation du partenaire est le 15e jour du mois. Le 1er juin 2018, le partenaire achète un nouvel abonnement. Le prix de l’abonnement est défini à 30 $ par licence par mois. Le 5 juin 2018, le partenaire suspend l’abonnement. Le 10 juin 2018, le partenaire réactive l’abonnement. Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin. 
- Crédit d’annulation de - 30 $ pour la période de service du 5 juin au 30 juin. Le crédit n’est pas calculé au prorata car l’abonnement a été suspendu au cours des 30 premiers jours. 
- Frais de 30 $ pour la période de service du 10 juin au 30 juin. Les frais ne sont pas calculés au prorata car l’abonnement a été réactivé au cours des 30 premiers jours. 

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |
|05/06/2018   |30/06/2018   |- 30 dollars   |1   |30 dollars   |Frais d'annulation |
|10/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais d'activation |

Notez que lorsqu'un abonnement est suspendu et réactivé, la date de renouvellement automatique reste à 12 mois à compter de la date d’achat d’origine.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Scénario 5B: Interrompre et réactiver après la date de facturation, mais moins de 30 jours à compter de la date d’achat

La date de facturation du partenaire est le 15e jour du mois. Le 1er juin 2018, le partenaire achète un nouvel abonnement. Le prix de l’abonnement est défini à 30 $ par licence par mois. Le 20 juin 2018, le partenaire suspend l'abonnement. Le 25 juin 2018, le partenaire réactive l’abonnement. Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin. 

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |

Le fichier de rapprochement du 15 juillet contiendra les lignes de facturation suivantes :
- Crédit d’annulation de - 30 $ pour la période de service du 20 juin au 30 juin. Le crédit n’est pas calculé au prorata car l’abonnement a été suspendu au cours des 30 premiers jours.
- Frais de 30 $ pour la période de service du 25 juin au 30 juin. Les frais ne sont pas calculés au prorata car l’abonnement a été réactivé au cours des 30 premiers jours.
- Frais de 30 $ pour la période de service du 1er juillet au 31 juillet.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |- 30 dollars   |1   |- 30 dollars   |Frais d'annulation |
|25/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais d'activation |
|01/07/2018   |31/07/2018   |30 dollars   |1   |30 dollars   |Frais de cycle |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Scénario 5C: Suspendre et réactiver (quantité de licences différente) après la date de facturation mais inférieure à 30 jours à compter de la date d’achat

La date de facturation du partenaire est le 15e jour du mois. Le 1er juin 2018, le partenaire achète un nouvel abonnement. Le prix de l’abonnement est défini à 30 $ par licence par mois. Le 20 juin 2018, le partenaire suspend l'abonnement. Le 25 juin 2018, le partenaire réactive l’abonnement avec deux licences. Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin. 

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |

Le fichier de rapprochement du 15 juillet contiendra les lignes de facturation suivantes :
- Crédit d’annulation de - 30 $ pour la période de service du 20 juin au 30 juin. Le crédit n’est pas calculé au prorata car l’abonnement a été suspendu au cours des 30 premiers jours.
- Frais de 30 $ pour la période de service du 25 juin au 30 juin. Les frais de réactivation ne sont pas calculés au prorata car l’abonnement a été réactivé au cours des 30 premiers jours. Les frais sont également basés sur la quantité de licences d’origine (1).
- Crédit de - 6 $ pour la période de service du 25 juin au 30 juin. Des frais de réactivation ne vous ont été facturés que pour 1 licence au cours de la période de service allant du 25 au 30 juin, où vous aviez 2 licences. Le crédit de -6 $ annule les frais de service incorrects facturés pour la période du 25 au 30 juin.
- Refacturation au prorata de 12 $ pour la période de service du 25 juin au 30 juin. Le partenaire a 2 licences pendant cette période de service. Le prix unitaire est calculé comme suit : (30/30)*6*2 = 12 $.
- Frais de 60 $ pour la période de service du 1er juillet au 31 juillet.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |- 30 dollars   |1   |- 30 dollars   |Frais d'annulation |
|25/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais d'activation |
|25/06/2018   |30/06/2018   |\- 6 $   |1   |\- 6 $   |Instance de cycle au prorata |
|25/06/2018   |30/06/2018   |6 dollars   |2   |12 dollars   |Instance de cycle au prorata |
|01/07/2018   |31/07/2018   |30 dollars   |2   |60 dollars   |Frais de cycle |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Scénario 6: Suspension de l’abonnement moins de 30 jours après l’achat et la réactivation plus de 30 jours après l’achat 

La date de facturation du partenaire est le 15e jour du mois. Le 1er juin, le partenaire achète un nouvel abonnement d'une licence à 30 dollars par mois. Le 5 juin, le partenaire suspend l'abonnement. Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin
- Crédit d’annulation de - 30 $ pour la période de service du 5 juin au 30 juin. Le crédit n’est pas calculé au prorata car l’abonnement a été suspendu au cours des 30 premiers jours.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat
|05/06/2018   |30/06/2018   |- 30 dollars   |1   |- 30 dollars   |Frais d'annulation

Le 10 juillet, le partenaire réactive l’abonnement. Le fichier de rapprochement du 15 juillet contiendra les lignes de facturation suivantes :

- Frais de réactivation de 21,30 $ pour la période de service du 10 juillet au 31 juillet. Les réactivations effectuées après les 30 jours qui suivent la date d’achat donnent lieu à des frais calculés au prorata. 

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/07/2018   |31/07/2018   |21,30 dollars   |1   |21,30 dollars   |Frais d'activation |

Le fichier de rapprochement du 15 août contiendra les lignes de facturation suivantes :
- Frais de 30 $ pour la période de service du 1er août au 31 août.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/08/2018   |30 dollars   |1   |30 dollars   |Frais de cycle |

Notez que lorsqu'un abonnement est suspendu et réactivé, la date de renouvellement automatique reste à 12 mois à compter de la date d’achat d’origine. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Scénario 7 : suspension et réactivation de l'abonnement plus de 30 jours après l’achat 
La date de facturation du partenaire est le 15e jour du mois. Le 1er juin, le partenaire achète un nouvel abonnement d'une licence à 30 dollars par mois. 

Le fichier de rapprochement du 15 juin contiendra uniquement les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |

Le partenaire suspend l’abonnement le 5 juillet mais le réactive le 15 juillet. Le fichier de rapprochement du 15 juillet contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1 juillet au 31 juillet.
- Crédit d’annulation de - 26,14 $ pour la période de service du 5 juillet au 31 juillet. Les annulations effectuées après les 30 jours qui suivent la date d’achat donnent lieu à un crédit calculé au prorata. Calcul = (prix mensuel/jours dans la période de service totale) x jours dans la période de service au prorata x quantité de licences x (- 1) = (30/31) x 27 x 1 x (- 1) = - 26,14.
- $16,45 frais de réactivation pour la période de service du 15 juillet au 31 juillet. Les réactivations effectuées après les 30 jours qui suivent la date d’achat donnent lieu à des frais calculés au prorata. Calcul = (30/31) x 17 x 1 = 16,45.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/07/2018   |31/07/2018   |30 dollars  |1   |30 dollars   |Frais de cycle |
|05/07/2018   |31/07/2018   |   - 26,14 dollars   |1   |- 26,14 dollars|Frais d'annulation |
|7/15/2018   |31/07/2018   |-$16,45   |1   |$16,45|Frais d'activation |

Le fichier de rapprochement du 15 août contient les indications suivantes :
- Frais de 30 $ pour la période de service du 1er août au 31 août.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/08/2018   |30 dollars  |1   |30 dollars   |Frais de cycle |

### <a name="scenario-8-change-of-license-quantity"></a>Scénario 8: Modification de la quantité de licences 

La date de facturation du partenaire est le 15. Le 1er juin, le partenaire achète un nouvel abonnement à 30 dollars par mois. Le 10 juin, le partenaire augmente la quantité de licences pour passer de 1 à 2 licences. Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin. Même si le partenaire a augmenté le nombre de licences avant la date de facturation du 15 juin, le système de facturation Microsoft ne prend pas en compte cette modification avant le jour anniversaire de l’abonnement le 1er juillet.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |

Le 1er juillet, le jour anniversaire de l'abonnement, le système de facturation Microsoft prend en compte le fait que le nombre de licences a été modifié pour passer de 1 à 2 le 10 juin. Le système de facturation génère un crédit et des refacturations au prorata pour la période de service entre le 1er juin et le 9 juin et entre le 10 juin et le 30 juin. 

Le fichier de rapprochement du 15 juillet contient les indications suivantes :

- Crédit de - 30 $ pour la période de service du 1er au 30 juin.
- Refacturation au prorata de 9 $ pour la période de service du 1 juin au 9 juin. Il s’agit de la période correspondant au moment où le client avait 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (30/30) x 9 x 1 = 9.
- Refacturation au prorata de 42 $ pour la période de service du 10 juin au 30 juin. Il s’agit de la période correspondant au moment où le client avait 2 licences. Calcul = (30/30) x 21 x 2 = 42.
- Frais de 60 $ pour la période de service du 1er juillet au 31 juillet.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |- 30 dollars   |1   |- 30 dollars|Instance de cycle au prorata |
|01/06/2018   |09/06/2018   |9 dollars   |1   |9 dollars|Instance de cycle au prorata |
|10/06/2018   |30/06/2018   |21 dollars   |2   |42 dollars|Instance de cycle au prorata |
|01/07/2018   |31/07/2018   |30 dollars   |2   |60 dollars   |Frais de cycle |

### <a name="scenario-9-add-on-subscriptions"></a>Scénario 9: Abonnements complémentaires

La date de facturation du partenaire est le 15e jour du mois. Le 1er juin, le partenaire achète un nouvel abonnement d'une licence à 30 dollars par mois. Le 10 juin, le partenaire achète un nouvel abonnement au module complémentaire à 5 dollars par mois. La date de renouvellement de l’abonnement au module complémentaire sera ajustée sur la date de renouvellement de l’abonnement de base qui est le 1er juin. 

Le 10 juin, le partenaire achète un abonnement au module complémentaire d'une licence à 5 dollars par mois. 

Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin. Cela concerne l’abonnement de base.
- Frais au prorata de 3,50 $ pour la période de service du 10 juin au 30 juin. Cela concerne l’abonnement au module complémentaire. 

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |30 dollars   |1   |30 dollars   |Frais au prorata à l'achat |
|10/06/2018   |30/06/2018   |3,50 dollars   |1   |3,50 dollars   |Frais au prorata à l'achat |

Le fichier de rapprochement du 15 juillet contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juillet au 31 juillet. Cela concerne l’abonnement de base.
- Frais de 5 $ pour la période de service du 1er juillet au 31 juillet. Cela concerne l’abonnement au module complémentaire.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|01/07/2018   |31/07/2018   |30 dollars   |1   |30 dollars   |Frais de cycle |
|01/07/2018   |31/07/2018   |5 dollars   |1   |5 dollars   |Frais de cycle |

Notez que la date de renouvellement automatique de l’abonnement au module complémentaire sera le 1er juin 2019, ce qui correspond à l’abonnement de base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Scénario 10: Nouvel achat le 29, le 30 ou le 31 

La date de facturation du partenaire est le 15e jour du mois. Le 29 mai, le partenaire achète un nouvel abonnement d'une licence à 30 dollars par mois. Les abonnements achetés le 29, le 30 ou le 31 auront une période gratuite entre la date d'achat et le 1er jour du mois suivant. Le jour anniversaire de l'abonnement sera le 1er par défaut. Dans ce scénario, l’abonnement bénéficient d'une période gratuite entre le 29 mai et le 31 mai et la période payante de 12 mois commence le 1er juin. 

Le fichier de rapprochement du 15 juin contiendra les lignes de facturation suivantes :

- Frais de 30 $ pour la période de service du 1er juin au 30 juin.

|**Début de la facturation**   |**Fin de la facturation**   |**Prix unitaire**   |**Spécifiée**   |**Proportion**   |**Type de frais** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29/05/2018   | 30/06/2018   |30 dollars   |1   |30 dollars  |Frais au prorata à l'achat |

Notez que l’abonnement sera renouvelé automatiquement le 1er juin 2019.
