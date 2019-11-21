---
title: Confirmer l'acceptation du contrat Microsoft Cloud par le client | Espace partenaires
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment confirmer l’acceptation par le client du contrat de Microsoft Cloud. Cela peut être nécessaire pour commander les produits et services Microsoft pour les clients.
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, MCA, Microsoft Cloud contrat, modèles de contrat client
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252589"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmer l'acceptation du contrat Microsoft Cloud par le client

**S’applique à**
-  Espace partenaires

> [!NOTE]
> La ressource d’accord est actuellement prise en charge par l’espace partenaires dans le cloud public Microsoft uniquement. Elle ne s’applique pas aux éléments suivants :
> * Espace partenaires géré par 21Vianet
> * Espace partenaires de Microsoft Cloud Germany
> * Espace partenaires de Microsoft Cloud for US Government

>[!NOTE]
>Le présent contrat est valable jusqu’au 31 janvier 2020. Après cette date, tous les clients, nouveaux et existants, doivent signer le nouveau contrat de client Microsoft. Pour en savoir plus, consultez [confirmer l’acceptation du client du contrat de client Microsoft](confirm-customer-agreement.md).

En tant que partenaire, vous devez obtenir l’acceptation par le client de l’accord de Microsoft Cloud avant de pouvoir commander des produits et services Microsoft pour ce client. Pour mieux aider les partenaires à répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l'acceptation en fournissant les informations suivantes sur la personne qui a accepté le contrat : 

-   Prénom

-   Nom

-   Adresse électronique

-   Numéro de téléphone (facultatif)

-   Date d’acceptation

Pour plus d’informations, consultez le contrat de Microsoft Cloud la confirmation de l’acceptation du client-Forum [aux questions](https://docs.microsoft.com/partner-center/confirm-consent-faq).

Les partenaires de facturation directe et les fournisseurs indirects doivent confirmer l’acceptation par le client de l’accord de Microsoft Cloud lors de la transmissions via l’espace partenaires ou l’API de l’espace partenaires. La confirmation est *obligatoire*.

Si la confirmation n’est pas fournie pour un client donné :

-   Vous ne pouvez pas créer de nouvelles commandes pour ce client.

-   Vous ne pouvez pas modifier le nombre de sièges des abonnements basés sur les sièges existants pour ce client.

La confirmation de l’acceptation du client peut être effectuée via l’espace partenaires ou l’API de l’espace partenaires. Pour effectuer cette opération via l’API espace partenaires, consultez les rubriques suivantes : 

-   [Recevoir la confirmation du consentement du client](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Récupérer les métadonnées de l’accord](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirmer le consentement du client](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Cela s’applique à la fois aux environnements de production et aux environnements sandbox.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmation de l’acceptation du client dans l’espace partenaires

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmer l’acceptation par un nouveau client

Utilisez la procédure suivante pour confirmer l’acceptation du client lors de la création d’un locataire client dans l’espace partenaires. Notez que vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **clients**, puis **nouveau client** , puis sélectionnez **informations sur le compte**.
2. Entrez les informations sur la **Société** et le **Contact principal**.

![Informations sur la société](images/mca/mca1.png)

3. Sous **Contrat Microsoft Cloud**, sélectionnez **Le client a accepté le dernier contrat Microsoft Cloud**.
4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.
5. Entrez les détails de l’utilisateur qui a fourni l’acceptation.

![Ajouter une date d’acceptation](images/mca/MCA3.png)

Par défaut, les informations d’utilisateur du contact principal sont affichées. Si ce n’est pas correct, sélectionnez **mettre à jour** , puis entrez le **prénom**, le **nom**, l' **adresse e-mail**et le*numéro de téléphone* (facultatif) de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmer l’acceptation par un client existant

Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.
2. Sélectionnez **Informations sur le compte**.
3. Sous **Contrat Microsoft Cloud**, sélectionnez **Mettre à jour**.

![Mettre à jour/Mise à jour](images/mca/mca4.png)

4. Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.
5. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.
6. Sélectionnez **Enregistrer et continuer**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmer l’acceptation du client lors de la création d'une nouvelle commande pour un client existant

Si vous essayez de créer une commande pour un client existant que vous n’avez pas confirmé précédemment, vous recevrez une invite pour terminer la confirmation. Utilisez la procédure suivante pour ce faire.

1. Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.
2. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.
3. Sélectionnez **Enregistrer et continuer**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Récupérer la confirmation de l’acceptation d'un client existant

Vous pouvez récupérer la confirmation de l’acceptation d'un client existant que vous avez fournie précédemment à l’aide de la procédure ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.
2. Sélectionnez **Informations sur le compte**.
3. Dans le cadre de l' **accord de Cloud Microsoft**, vous verrez si une confirmation a été fournie pour ce client.
