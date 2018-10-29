---
title: Migrer des abonnements Dynamics AX vers Dynamics&nbsp;365 | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Microsoft propose Dynamics365, la nouvelle génération d’applications métier intelligentes permettant à votre entreprise de se développer, croître et se transformer pour répondre aux besoins de vos clients et saisir de nouvelles opportunités.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e992a3cdfc0bbb01a303a8b00bfeda3cf60d1882
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5797132"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrer des abonnements DynamicsAX vers Dynamics365

**S'applique à**

-  Espace partenaires

Microsoft propose Dynamics365, la nouvelle génération d’applications métier intelligentes permettant à votre entreprise de se développer, croître et se transformer pour répondre aux besoins de vos clients et saisir de nouvelles opportunités. Dans le cadre du nouveau produit, Microsoft présente les nouvelles formules d’abonnement Microsoft Dynamics pour les clients le 1ernovembre2016, qui sont similaires, mais pas identiques à vos formules actuelles.

Les instructions fournies dans ce document décrivent comment les fournisseurs indirects peuvent transformer les abonnements Microsoft DynamicsAX et Microsoft Dymanics CRM Online des clients en nouveaux abonnements Microsoft Dynamics365. Elles s’appliquent également aux autres produits Microsoft qui connaissent des mises à jour, obligeant les fournisseurs à migrer les abonnements des clients vers une nouvelle référence (SKU).

Les formules MicrosoftDynamics CRM Online et AX sont retirées.  À partir du 1erjuillet2017, vous ne pouvez plus renouveler d'abonnement dans les formules anciennes, et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration.

Lorsque les abonnements CRM Online et AX prendront fin, ils seront annulés. Pour garantir la continuité des activités pour les clients, vous devez passer les clients ayant des abonnements arrivant à expiration à une option de référence (SKU) prise en charge, répertoriée ci-dessous. Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d’abonnement annuelle afin de leur éviter toute interruption de service. 

Sur la page des détails de ces abonnements qui arrivent à expiration, le statut de l'abonnement «Renouvellements automatiques le [date]» est remplacé par «Expire le [date]». 

Si vous utilisez l’API (CREST ou Espace partenaires), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec la propriété de renouvellement automatique = False. Les abonnements ont été définis sur renouvellement automatique = False le 1er juillet2017. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

**Modifications des licences Microsoft DynamicsAX**

La gamme de produits Microsoft DynamicsAX n’est plus disponible à partir du 1ernovembre2016. Pour en savoir plus sur les nouvelles options de licence de Dynamics365, consultez le [Guide des licences](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).

 Pour plus d’informations sur le mappage de licences, consultez le tableau suivant:

|**SKU retirée**   |**SKU Dynamics365**   |
|-------------------|:----------------------|
|SKU Entreprise|Formule MicrosoftDynamics365 for Unified Operations ou Microsoft Dynamics365 |
|Tâche|MicrosoftDynamics365 for Activity
|Tâche/libre-service|Microsoft Dynamics365 for Team Members|
|Appareil|Appareil Microsoft Dynamics365 for Operations|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Modifications des licences Microsoft Dynamics CRM Online 

**Microsoft Dynamics CRM Online**

La formule Microsoft Dynamics CRM Online actuelle n’est plus disponible depuis le 1ernovembre2016. Pour en savoir plus sur les nouvelles options de licence de Microsoft Dynamics365, consultez le [Guide des licences](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Pour en savoir plus sur les nouvelles options de gestion de licences, consultez [Informations importantes pour les clients de CRM Online](https://go.microsoft.com/fwlink/?linkid=831667).

Pour plus d’informations sur le mappage de licences, consultez le tableau suivant:

|**SKU retirée**   |**SKU Dynamics365**   |
|-------------------|:----------------------|
|Entreprise|Formule Dynamics365 Enterprise Customer Engagement |
|Professionnel|Formule Dynamics365 Enterprise Customer Engagement, Dynamics365 for Sales ou Dynamics365 for Customer Service|
|De base|Dynamics365 for Team Members, Dynamics365 for Sales, Dynamics365 for Customer Service ou formule Dynamics365 Enterprise Customer Engagement|
|Essentiel|Dynamics365 for Team Members|
|Extension Field service|Formule Dynamics 365 Enterprise Customer Engagement ou Dynamics365 for Field Service|
|Extension Project Service Automation|Formule Dynamics365 Customer Engagement ou Dynamics365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit


Microsoft offre en permanence de nouveaux produits et services aux revendeurs et fournisseurs. Dans ces cas, un revendeur peut avoir besoin de mettre à niveau les services de ses clients ou de migrer leurs abonnements à partir de références (SKU) qui vont progressivement disparaître. La migration de clients depuis des références anciennes vers des références plus récentes doit respecter la séquence suivante&nbsp;:

-   [Acheter le nouvel abonnement](#manual-subscription-migration-purchasenewsubsc)
-   [Réaffecter les licences utilisateur actuelles](#manual-subscription-migration-reassignlicenses)
-   [Annuler l’ancien abonnement](#manual-subscription-migration-cancelsubscriptions)

Dans les procédures suivantes, vous migrez un client de Microsoft Dynamics AX ou CRM Online vers Dynamics365.

Le revendeur doit migrer un client avec un abonnement DynamicsAX Enterprise vers un abonnement Dynamics365 for Operations. La première étape consiste à acheter Dynamics365 for Operations.  Répétez ces étapes pour un client CRM Online migrant vers MicrosoftDynamics365.

<a href="" id="purchasenewsubsc"></a>

**Acheter le nouvel abonnement**

1.  Dans le menu **Espace partenaires** , sélectionnez les **clients**, sélectionnez le client à déplacer et choisissez **d’Ajouter des abonnements**.
2.  Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, Dynamics&nbsp;365 for Operations, Enterprise Edition), indiquez le nombre de licences et choisissez **Envoyer**.

    Votre client doit maintenant avoir un ancien et un nouvel abonnement&nbsp;: dans cet exemple, l’ancien (Dynamics AX Enterprise) et le nouveau (Dynamics&nbsp;365 for Operations, Enterprise Edition).

<a href="" id="reassignlicenses"></a> L’étape suivante consiste à réaffecter toutes les licences utilisateur existantes au nouvel abonnement.

**Réaffecter les licences utilisateur**

1.  Dans le menu **Espace partenaires** , sélectionnez les **clients**, sélectionnez le client à déplacer et choisissez les **utilisateurs et licences**. La page Utilisateurs et licences du client s’ouvre.
2.  Pour réaffecter les licences utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.
3.  Dans la page **Gérer les licences**, désactivez la case à cocher de la licence **Dynamics AX Enterprise**, puis sélectionnez la licence **Dynamics 365 for Operations**.
4.  Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées.
5.  Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.

<a href="" id="cancelsubscriptions"></a> Une fois les licences utilisateur attribuées au nouveau service, vous pouvez en toute sécurité annuler l’ancien abonnement au premier niveau du client.

**Annuler l’ancien abonnement**

1.  Dans le menu **Espace partenaires** , sélectionnez les **clients**, sélectionnez le client à déplacer et sélectionnez l’abonnement à annuler.
2.  Dans la page de détails de l’abonnement, sélectionnez **Suspendu** dans **État**.
3.  Sélectionnez **Envoyer**.

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est automatiquement désapprovisionné après 120&nbsp;jours. Aucun frais n’est facturé au client pour l’ancien abonnement.

## <a name="additional-considerations"></a>Autres éléments à prendre en considération


Si votre client passe du programme Open Channel au programme Cloud Services pour approvisionner davantage d’abonnements, vous devrez également migrer ses abonnements&nbsp;:

-   Si le client a reçu son ancien abonnement via le programme Open Channel, la transition vers le programme Fournisseur de services Cloud sur la nouvelle référence (SKU) est simple.
-   Si le client n’est pas encore votre client, vous pouvez l’inviter. Pour plus d’informations, consultez la rubrique d’aide [Demander une relation avec un client](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Lorsque le client vous accepte comme fournisseur indirect, la procédure d’approvisionnement reste essentiellement la même&nbsp;: vous achetez le nouvel abonnement, puis vous affectez les licences utilisateur. La seule différence concerne l’annulation du ou des anciens abonnements. Un nouveau fournisseur ne peut pas annuler ou suspendre des abonnements souscrits par le biais d’autres canaux. Si le client a souscrit des abonnements via un autre canal de vente, comme le programme Open Channel, il doit les annuler lui-même dans ce canal.

 

 



