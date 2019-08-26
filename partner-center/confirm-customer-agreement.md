---
title: Confirmer l’acceptation du contrat client Microsoft par le client | Espace partenaires
ms.topic: article
ms.date: 04/16/2019
Description: En tant que partenaire, vous devez obtenir l’acceptation du contrat client Microsoft par le client pour pouvoir lui commander des produits et des services Microsoft. Pour mieux aider les partenaires à répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l'acceptation en fournissant des informations sur la personne qui a accepté le contrat.
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, MCA, Contrat Microsoft Cloud, Contrat client Microsoft, modèles de contrat client
ms.localizationpriority: medium
ms.openlocfilehash: 295c997baa43dd087552315d71d726a0f28c6ed1
ms.sourcegitcommit: 0712e68734f0b3e53821b490a6c32a6c991a6e49
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/21/2019
ms.locfileid: "69871772"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Confirmer l’acceptation du contrat client Microsoft par le client (préversion)

Actuellement, avant qu’un partenaire CSP puisse passer une commande au nom d’un client, le client doit accepter et signer le **contrat Microsoft Cloud** applicable. Ensuite, le partenaire doit confirmer l’acceptation du contrat par le client en fournissant des informations sur le signataire à Microsoft. Si un client ne confirme pas son acceptation du contrat Microsoft Cloud :
- Vous ne pourrez pas créer de commandes pour ce client.
- Vous ne pourrez pas modifier le nombre de sièges des abonnements existants basés sur les utilisateurs pour ce client.

Pour plus d’informations sur la façon de confirmer l’acceptation par un client du contrat Microsoft Cloud à l’aide du tableau de bord ou de l’API de l’Espace partenaires, consultez [Confirmer l'acceptation du contrat Microsoft Cloud par le client](confirm-consent.md).

Le 1er octobre 2019, Microsoft présentera le **contrat client Microsoft** au programme CSP pour remplacer le contrat Microsoft Cloud. Pour faciliter la migration des partenaires vers le nouveau contrat, le contrat Microsoft Cloud actuel sera pris en charge dans le programme CSP jusqu’au 31 janvier 2019. Pour plus d’informations sur la chronologie, consultez le tableau suivant :

| Date | Jalon | Détails |
|------------|------------|--------------------------------|
|1er août 2019|Aperçu de l’expérience utilisateur disponible dans le bac à sable|Les partenaires peuvent confirmer l’acceptation par le client du contrat client Microsoft à l’aide du tableau de bord de l’Espace partenaires dans l’environnement du bac à sable (sandbox) CSP. Les partenaires ayant accès à l’environnement du bac à sable (sandbox) CSP peuvent afficher un aperçu des modifications de l’expérience utilisateur. Les partenaires sans accès au bac à sable peuvent en savoir plus sur les modifications apportées dans cette rubrique.|
|2 septembre 2019|L’aperçu de l’API est disponible dans le bac à sable.|Le partenaire peut confirmer l’acceptation par le client du contrat client Microsoft à l’aide du l’API de l’Espace partenaires dans l’environnement du bac à sable (sandbox) CSP. Les partenaires de l’API peuvent utiliser cette opportunité pour afficher un aperçu des modifications de l’API et commencer à travailler sur l’intégration de l’API pour prendre en charge le nouveau contrat.|
|1er octobre 2019|Contrat client Microsoft disponible en production|Microsoft présente le contrat client Microsoft au programme CSP pour remplacer le contrat Microsoft Cloud. Les partenaires peuvent confirmer l’acceptation par le client du contrat client Microsoft à l’aide de l’API et du tableau de bord de l’Espace partenaires en production. Le contrat Microsoft Cloud reste pris en charge dans le programme partenaire CSP. Toutefois, les partenaires sont invités à commencer à migrer vers le contrat client Microsoft. Les nouveaux achats et les modifications apportées au nombre de sièges dans les abonnements existants nécessitent la confirmation par le partenaire du contrat client Microsoft ou du contrat Microsoft Cloud. Certaines nouvelles offres (par exemple, le nouveau plan Azure) requièrent la confirmation du contrat client Microsoft.|
|31 janvier 2019|Contrat Microsoft Cloud supprimé de la production|Le contrat Microsoft Cloud n’est plus accepté dans le programme partenaire CSP. Les nouveaux achats et les modifications apportées au nombre de sièges dans les abonnements existants nécessitent la confirmation par le partenaire du contrat client Microsoft. Cette exigence s’applique aux nouveaux clients et aux clients existants qui ont peut-être déjà accepté le contrat Microsoft Cloud.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmer l’acceptation par les nouveaux clients

Lorsque vous créez un locataire client dans l’Espace partenaires, suivez les étapes ci-dessous pour confirmer l’acceptation par le client du contrat client Microsoft. Vous devez être Agent administrateur ou Commercial pour suivre ces étapes.

1. Sélectionnez **Clients**, puis **Nouveau client**.

2. Sous **Informations sur le compte**, entrez les informations relatives à l’entreprise et à son contact principal.

3. Sous **Contrat Microsoft**, sélectionnez le **Contrat client Microsoft**.

4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Assurez-vous que les coordonnées de l’utilisateur principal affichées sont correctes. Si elles ne sont pas correctes, sélectionnez **Mettre à jour**, puis saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

![Nouveau client](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmer l’acceptation par les clients existants

Vous devez être Agent administrateur ou Commercial pour effectuer cette opération :

1. Sélectionnez **Clients**. Recherchez et sélectionnez le client.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.

4. Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Sélectionnez **Enregistrer** et continuez.

![Client existant](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Récupérer la confirmation de l’acceptation par le client

Vous pouvez récupérer la confirmation qu’un client existant a accepté le contrat client Microsoft en suivant les étapes ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, vérifiez si la confirmation a été fournie ou n’a pas été fournie par ce client.


