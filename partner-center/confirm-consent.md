---
title: Confirmer que le client a accepté le Contrat client Microsoft
description: Découvrez comment confirmer l’acceptation du Contrat client Microsoft par les clients. Cela peut être nécessaire pour commander des produits et services Microsoft pour les clients.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354608"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Mise à jour de la méthode permettant de confirmer l’acceptation du Contrat client Microsoft par les clients


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

- Vous ne pourrez pas créer de commandes pour ce client.

- Vous ne pourrez pas changer le nombre de licences des abonnements existants basés sur les licences pour ce client.

La confirmation de l’acceptation du client peut être effectuée par le biais de l’Espace partenaires ou de l’API de l’Espace partenaires. Pour effectuer cette opération via l’API de l’Espace partenaires, consultez les rubriques suivantes :

- [Obtenir la confirmation du consentement du client](/partner-center/develop/get-confirmation-of-customer-consent)

- [Obtenir les métadonnées d’un contrat](/partner-center/develop/get-agreement-metadata)

- [Confirmer le consentement du client](/partner-center/develop/confirm-customer-consent)

Cela s’applique à la fois aux environnements de production et aux environnements de bac à sable (sandbox).

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmer l’acceptation par un nouveau client

Utilisez la procédure suivante pour confirmer l’acceptation du client quand vous créez un locataire du client dans l’Espace partenaires. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, **Nouveau client**, puis **Informations sur le compte**.

2. Entrez les informations relatives à la **Société** et au **Contact principal**.

   :::image type="content" source="images/mca/mca1.png" alt-text="Informations sur la société":::

3. Sous **Contrat client Microsoft**, sélectionnez **Le client a accepté le dernier Contrat client Microsoft**.

4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Entrez les détails de l’utilisateur qui a fourni l’acceptation.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Ajouter une date d’acceptation":::

   Par défaut, les informations d’utilisateur du contact principal sont affichées. Si elles ne sont pas correctes, sélectionnez **Mettre à jour**, puis entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone* (facultatif) de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmer l’acceptation par un client existant

Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.

   :::image type="content" source="images/mca/mca4.png" alt-text="Mettre à jour":::

4. Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.

5. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

6. Sélectionnez **Enregistrer et continuer**.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmer l’acceptation du client lors de la création d’une commande pour un client existant

Si vous essayez de créer une commande pour un client existant que vous n’avez pas encore confirmé, vous recevrez une invite pour effectuer la confirmation. Pour ce faire, utilisez la procédure suivante.

1. Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.

2. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

3. Sélectionnez **Enregistrer et continuer**.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Récupérer la confirmation de l’acceptation d’un client existant

Vous pouvez récupérer la confirmation de l’acceptation d’un client existant que vous avez fournie précédemment à l’aide de la procédure ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, vous voyez si la confirmation a été fournie, ou non, pour ce client.

## <a name="next-steps"></a>Étapes suivantes

- [Confirmer l’acceptation du Contrat client Microsoft par le client dans le cadre du programme des partenaires fournisseurs de solutions Cloud](confirm-customer-agreement.md)

- [Attester l’acceptation du Contrat client Microsoft au nom de votre client](attest-acceptance-customer-agreement.md)