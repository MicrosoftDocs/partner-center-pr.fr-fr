---
title: Confirmer l’acceptation du Contrat client Microsoft par les clients
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment confirmer l’acceptation du Contrat client Microsoft par les clients. Cela peut être nécessaire pour commander des produits et services Microsoft pour les clients.
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, MCA, Contrat client Microsoft, modèles de contrat client
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d45f04c8ee1a8d8715f5c6484598ecaca83b1f1
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908147"
---
# <a name="overview-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Vue d'ensemble : Confirmer l’acceptation du Contrat client Microsoft par les clients

**S’applique à**
-  Espace partenaires

**Rôles appropriés**

- Agent d’administration
- Agent commercial

> [!NOTE]
> La ressource Contrat est actuellement prise en charge par l’Espace partenaires dans le cloud public Microsoft uniquement. Elle n’est pas applicable aux éléments suivants :
> * Espace partenaires géré par 21Vianet
> * Espace partenaires de Microsoft Cloud Germany
> * Espace partenaires de Microsoft Cloud for US Government

>[!NOTE]
>À compter du 31 janvier 2020, tous les clients, nouveaux et existants, doivent signer le nouveau Contrat client Microsoft. Pour en savoir plus, consultez [Confirmer l’acceptation du Contrat client Microsoft par les clients](confirm-customer-agreement.md).

En tant que partenaire, vous devez obtenir l’acceptation du Contrat client Microsoft par le client pour pouvoir lui commander des produits et des services Microsoft. Pour permettre aux partenaires à mieux répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l’acceptation en fournissant les informations suivantes sur la personne qui a accepté le contrat :

- Prénom

- Nom

- Adresse de messagerie

- Numéro de téléphone (facultatif)

- Date d’acceptation

Les partenaires associés à une facturation directe et les fournisseurs indirects peuvent confirmer l’acceptation du Contrat client Microsoft par le client quand ils effectuent des transactions par le biais de l’Espace partenaires ou de l’API de l’Espace partenaires. La confirmation est *obligatoire*.

Si la confirmation n’est pas fournie pour un client donné :

-    Vous ne pourrez pas créer de commandes pour ce client.

-    Vous ne pourrez pas changer le nombre de sièges des abonnements existants basés sur les sièges pour ce client.

La confirmation de l’acceptation du client peut être effectuée par le biais de l’Espace partenaires ou de l’API de l’Espace partenaires. Pour effectuer cette opération via l’API de l’Espace partenaires, consultez les rubriques suivantes : 

-   [Obtenir la confirmation du consentement du client](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Obtenir les métadonnées d’un contrat](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirmer le consentement du client](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Cela s’applique à la fois aux environnements de production et aux environnements de bac à sable (sandbox).

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmation de l’acceptation du client dans l’Espace partenaires

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmer l’acceptation par un nouveau client

Utilisez la procédure suivante pour confirmer l’acceptation du client quand vous créez un locataire du client dans l’Espace partenaires. Notez que vous devez être Agent d’administration ou Agent commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, **Nouveau client**, puis **Informations sur le compte**.
2. Entrez les informations relatives à la **Société** et au **Contact principal**.

![Informations sur la société](images/mca/mca1.png)

3. Sous **Contrat client Microsoft**, sélectionnez **Le client a accepté le dernier Contrat client Microsoft**.
4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.
5. Entrez les détails de l’utilisateur qui a fourni l’acceptation.

![Ajouter une date d’acceptation](images/mca/MCA3.png)

Par défaut, les informations d’utilisateur du contact principal sont affichées. Si elles ne sont pas correctes, sélectionnez **Mettre à jour**, puis entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone* (facultatif) de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmer l’acceptation par un client existant

Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.
2. Sélectionnez **Informations sur le compte**.
3. Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.

![Mettre à jour/Mise à jour](images/mca/mca4.png)

4. Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.
5. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.
6. Sélectionnez **Enregistrer et continuer**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmer l’acceptation du client lors de la création d’une commande pour un client existant

Si vous essayez de créer une commande pour un client existant que vous n’avez pas encore confirmé, vous recevrez une invite pour effectuer la confirmation. Pour ce faire, utilisez la procédure suivante.

1. Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.
2. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.
3. Sélectionnez **Enregistrer et continuer**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Récupérer la confirmation de l’acceptation d’un client existant

Vous pouvez récupérer la confirmation de l’acceptation d’un client existant que vous avez fournie précédemment à l’aide de la procédure ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.
2. Sélectionnez **Informations sur le compte**.
3. Sous **Contrat client Microsoft**, vous voyez si la confirmation a été fournie, ou non, pour ce client.
