---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. Dans le cadre du nouveau produit, Microsoft présente les nouvelles formules d’abonnement Microsoft Dynamics pour les clients le 1ernovembre2016, qui sont similaires, mais pas identiques à vos formules actuelles.

Les instructions fournies dans ce document décrivent comment les fournisseurs indirects peuvent transformer les abonnements Microsoft DynamicsAX et Microsoft Dymanics CRM Online des clients en nouveaux abonnements Microsoft Dynamics365. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

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


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [Annuler l’ancien abonnement](#manual-subscription-migration-cancelsubscriptions)

Dans les procédures suivantes, vous migrez un client de Microsoft Dynamics AX ou CRM Online vers Dynamics365.

Le revendeur doit migrer un client avec un abonnement DynamicsAX Enterprise vers un abonnement Dynamics365 for Operations. La première étape consiste à acheter Dynamics365 for Operations.  Répétez ces étapes pour un client CRM Online migrant vers MicrosoftDynamics365.

<a href="" id="purchasenewsubsc"></a>

**Acheter le nouvel abonnement**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



