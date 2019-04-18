---
title: Confirmer l'acceptation du contrat Microsoft Cloud par le client | Espace partenaires
ms.topic: article
ms.date: 04/16/2019
Description: En tant que partenaire, vous devez obtenir l’acceptation du contrat Microsoft Cloud par le client pour pouvoir lui commander des produits et des services Microsoft. Pour mieux partenaires répondent aux exigences de conformité, Microsoft vous demande de partenaires pour confirmer l’acceptation en fournissant certains détails concernant la personne qui a accepté le contrat.
author: LauraBrenner
ms.author: v-petand
keywords: client, les clients, donner son consentement, MCA, accord du Cloud Microsoft, modèles de contrat de client
ms.localizationpriority: medium
ms.openlocfilehash: 9dad303b419f3dadd33f4937933638c60c45994b
ms.sourcegitcommit: 7022f1e3d26751e66f90db96bf6d881cb2a694d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/17/2019
ms.locfileid: "59652251"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmer l'acceptation du contrat Microsoft Cloud par le client

**S’applique à**
-  Espace partenaires

> [!NOTE]
> La ressource de l’accord est pris en charge par les partenaires dans le cloud public Microsoft uniquement. Il n’est pas applicable à :
> * Espace partenaires géré par 21Vianet
> * Espace partenaires de Microsoft Cloud Germany
> * Espace partenaires de Microsoft Cloud for US Government

En tant que partenaire, vous devez obtenir l’acceptation du contrat Microsoft Cloud par le client pour pouvoir lui commander des produits et des services Microsoft. Pour mieux aider les partenaires à répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l'acceptation en fournissant les informations suivantes sur la personne qui a accepté le contrat : 

-   Prénom

-   Nom

-   Adresse électronique

-   Numéro de téléphone (facultatif)

-   Date d’acceptation

Pour plus d’informations, consultez la confirmation de l’acceptation de client accord du Cloud Microsoft [Forum aux Questions](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

Partenaires de l’électronique et les fournisseurs indirects doivent confirmer l’acceptation du client de l’accord de Cloud de Microsoft lors des transactions via des partenaires ou des API espace partenaires. La confirmation est *obligatoire*.

Si la confirmation n’est pas fournie pour un client donné :

-   Vous ne pourrez pas créer de commandes pour ce client.

-   Vous ne pourrez pas modifier le nombre de sièges des abonnements existants basés sur les utilisateurs pour ce client.

Confirmation d’acceptation du client peut être effectuée par le biais de partenaires ou de l’API espace partenaires. Pour ce faire, via l’API espace partenaires, consultez les rubriques suivantes : 

-   [Obtenir la confirmation de consentement du client](https://docs.microsoft.com/en-us/partner-center/develop/get-confirmation-of-customer-consent)

-   [Obtenir les métadonnées de l’accord](https://docs.microsoft.com/en-us/partner-center/develop/get-agreement-metadata)

-   [Confirmer le consentement du client](https://docs.microsoft.com/en-us/partner-center/develop/confirm-customer-consent)


Cela vaut pour les environnements de bac à sable et de production.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmation d’acceptation du client dans l’espace partenaires

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmer l’acceptation par un nouveau client

Utilisez la procédure suivante pour confirmer l’acceptation du client lorsque vous créez un nouveau client dans l’espace partenaires. Notez que vous devez être Agent administrateur ou Commercial pour effectuer cette opération.
 
1.  Sélectionnez **clients**, puis **nouveau client** , puis sélectionnez **informations sur le compte**.

2.  Entrez les informations sur la **Société** et le **Contact principal**.

![Informations de l’entreprise](images/mca/mca1.png)

3.  Sous **Contrat Microsoft Cloud**, sélectionnez **Le client a accepté le dernier contrat Microsoft Cloud**. 

4.  Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5.  Entrez les détails de l’utilisateur qui a fourni l’acceptation. 

![Ajouter la date d’acceptation](images/mca/MCA3.png)

Par défaut, les informations d’utilisateur du contact principal sont affichées. Si elles ne sont pas correctes, sélectionnez **Mettre à jour**, puis saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone* (facultatif) de la personne qui a accepté le contrat.

6.  Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmer l’acceptation par un client existant

Vous devez être Agent administrateur ou Commercial pour effectuer cette opération. 

1.  Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher. 

2.  Sélectionnez **informations sur le compte**.

3.  Sous **Contrat Microsoft Cloud**, sélectionnez **Mettre à jour**.

![Mettre à jour/Mise à jour](images/mca/mca4.png)

4.  Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.

5.  Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

6.  Sélectionnez **Enregistrer et continuer**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmer l’acceptation du client lors de la création d'une nouvelle commande pour un client existant

Si vous essayez de créer une nouvelle commande pour un client existant que vous n’avez pas encore confirmée, vous recevrez une invite pour terminer la confirmation. Utilisez la procédure suivante pour ce faire. 

1.  Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.

2.  Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

3.  Sélectionnez **Enregistrer et continuer**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Récupérer la confirmation de l’acceptation d'un client existant

Vous pouvez récupérer la confirmation de l’acceptation d'un client existant que vous avez fournie précédemment à l’aide de la procédure ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération. 

1.  Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher. 

2.  Sélectionnez **informations sur le compte**.

3.  Sous **Contrat Microsoft Cloud**, vous verrez si la confirmation a été fournie ou non pour ce client.

