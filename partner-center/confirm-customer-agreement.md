---
title: Confirmer l’acceptation du client du contrat de la clientèle Microsoft | Espace partenaires
ms.topic: article
ms.date: 04/16/2019
Description: En tant que partenaire, vous devez obtenir l’acceptation du contrat du client Microsoft par le client avant de pouvoir commander des produits et services Microsoft pour ce client. Pour mieux aider les partenaires à répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l’acceptation en fournissant certains détails concernant la personne qui a accepté le contrat.
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, MCA, Microsoft Cloud contrat, contrat client Microsoft, modèles de contrat client
ms.localizationpriority: medium
ms.openlocfilehash: 6ca8eb3acdee0114f01dbd5952e9c092859147a2
ms.sourcegitcommit: ee722dc2b9d82557d273738b64cec6d8cb435084
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/31/2019
ms.locfileid: "68681755"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Confirmer l’acceptation du client du contrat de client Microsoft (version préliminaire)

Actuellement, avant qu’un partenaire CSP puisse passer une commande au nom d’un client, le client doit accepter et signer le **contrat de Microsoft Cloud**applicable. Ensuite, le partenaire doit confirmer son acceptation par le client en fournissant des informations sur le signataire à Microsoft. Si un client ne confirme pas son acceptation du contrat de Microsoft Cloud:
- Vous ne pourrez pas créer de commandes pour ce client.
- Vous ne pourrez pas modifier le nombre de sièges des abonnements existants basés sur les utilisateurs pour ce client.

Pour plus d’informations sur la façon de confirmer l’acceptation par un client du contrat de Microsoft Cloud à l’aide du tableau de bord ou de l’API de l’espace partenaires, consultez [confirmer l’acceptation du client du contrat de Microsoft Cloud](confirm-consent.md).

Le 1er octobre 2019, Microsoft présentera le **contrat du client Microsoft** au programme CSP pour remplacer le contrat de Microsoft Cloud. Pour faciliter la migration des partenaires vers le nouvel accord, le contrat de Microsoft Cloud actuel sera pris en charge dans le programme CSP jusqu’au 31 janvier 2019. Pour plus d’informations sur la chronologie, consultez le tableau suivant:

| Date | Jalon | Détails |
|------------|------------|--------------------------------|
|1er août 2019|Aperçu de l’expérience utilisateur disponible dans le bac à sable|Les partenaires peuvent confirmer l’acceptation par le client du contrat de client Microsoft à l’aide du tableau de bord de l’espace partenaires dans l’environnement du sandbox CSP. Les partenaires ayant accès à l’environnement du bac à sable (sandbox) CSP prévisualisent les modifications de l’expérience utilisateur. Les partenaires sans accès sandbox peuvent en savoir plus sur les modifications apportées à cette rubrique.|
|Le 02 septembre 2019|L’aperçu de l’API est disponible dans le bac à sable (sandbox).|Le partenaire peut confirmer l’acceptation par le client du contrat de client Microsoft à l’aide de l’API de l’espace partenaires dans l’environnement du sandbox CSP. Les partenaires API peuvent utiliser cette opportunité pour afficher un aperçu des modifications de l’API et commencer à travailler sur l’intégration des API pour prendre en charge le nouvel accord.|
|01 octobre 2019|Contrat client Microsoft disponible en production|Microsoft présente le contrat du client Microsoft au programme CSP pour remplacer le contrat de Microsoft Cloud. Les partenaires peuvent confirmer l’acceptation par le client du contrat de client Microsoft en utilisant le tableau de bord de l’espace partenaires et l’API en production. Le contrat de Microsoft Cloud reste pris en charge dans le programme partenaire CSP. Toutefois, les partenaires sont invités à commencer à migrer vers le contrat de la part du client Microsoft. Les modifications apportées aux nouveaux achats et au nombre de sièges dans les abonnements existants nécessitent la confirmation du partenaire du contrat de client Microsoft ou du contrat de Microsoft Cloud. Certaines nouvelles offres (par exemple, le nouveau plan Azure) requièrent la confirmation du contrat du client Microsoft.|
|31 janvier 2019|Contrat de Microsoft Cloud supprimé de la production|Le contrat de Microsoft Cloud n’est plus accepté dans le programme partenaire CSP. Les modifications apportées aux nouveaux achats et au nombre de sièges dans les abonnements existants obligent le partenaire à fournir une confirmation du contrat du client Microsoft. Cette exigence s’applique aux nouveaux clients et aux clients existants qui ont peut-être déjà accepté le contrat de Microsoft Cloud.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmer l’acceptation du client pour les nouveaux clients

Lorsque vous créez un locataire client dans l’espace partenaires, suivez les étapes ci-dessous pour confirmer l’acceptation par le client du contrat de client Microsoft. Pour exécuter ces étapes, vous devez être un agent d’administration ou un agent commercial.

1. Sélectionnez **Clients**, puis **Nouveau client**.

2. Sous **informations**sur le compte, entrez les informations relatives à la société et à son contact principal.

3. Sous **contrat Microsoft**, sélectionnez le **contrat client Microsoft**.

4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Assurez-vous que les informations de contact de l’utilisateur principal affichées sont correctes. Si ce n’est pas le cas, sélectionnez **mettre à jour** , puis entrez le **prénom**, le **nom**, l' **adresse de messagerie**et le **numéro de téléphone** (facultatif) de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

![Nouveau client](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmer l’acceptation du client pour les clients existants

Pour ce faire, vous devez être un agent d’administration ou un agent commercial:

1. Sélectionnez **clients**. Recherchez et sélectionnez le client.

2. Sélectionnez **informations sur le compte**.

3. Sous **contrat client Microsoft**, sélectionnez **mettre à jour**.

4. Entrez le **prénom**, le **nom**, l' **adresse de messagerie**et le **numéro de téléphone** (facultatif) de la personne qui a accepté le contrat. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Sélectionnez **Enregistrer** et continuer.

![Client existant](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Récupérer la confirmation de l’acceptation du client

Vous pouvez récupérer la confirmation qu’un client existant a accepté le contrat du client Microsoft en suivant les étapes ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **informations sur le compte**.

3. Sous **contrat de Cloud Microsoft**, affichez si la confirmation a été fournie ou n’a pas été fournie par ce client.


