---
title: Confirmer l’acceptation du contrat client Microsoft par le client | Espace partenaires
ms.topic: article
ms.date: 09/30/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: En tant que partenaire, vous devez obtenir l’acceptation du contrat du client Microsoft par le client avant de pouvoir commander des produits et services Microsoft pour ce client. Pour mieux aider les partenaires à répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l'acceptation en fournissant des informations sur la personne qui a accepté le contrat.
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, MCA, Contrat Microsoft Cloud, Contrat client Microsoft, modèles de contrat client
ms.localizationpriority: medium
ms.openlocfilehash: 8a4b28db2884f833b6df9ee0dd08f262afdb0888
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653645"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirmer l’acceptation du client du contrat de client Microsoft

Actuellement, avant qu’un partenaire CSP puisse passer une commande au nom d’un client, le client doit accepter et signer le **contrat de Microsoft Cloud**applicable. Ensuite, le partenaire doit confirmer l’acceptation du contrat par le client en fournissant des informations sur le signataire à Microsoft. À défaut de confirmation :
- Vous ne pouvez pas créer de nouvelles commandes pour ce client.
- Vous ne pouvez pas modifier le nombre de sièges des abonnements basés sur les sièges existants pour ce client.

Pour plus d’informations sur la façon de confirmer l’acceptation par un client du contrat Microsoft Cloud à l’aide du tableau de bord ou de l’API de l’Espace partenaires, consultez [Confirmer l'acceptation du contrat Microsoft Cloud par le client](confirm-consent.md).

Le 1er octobre 2019, Microsoft présentera le **contrat client Microsoft** au programme CSP pour remplacer le contrat Microsoft Cloud. Pour faciliter la migration des partenaires vers le nouveau contrat, le contrat Microsoft Cloud actuel sera pris en charge dans le programme Fournisseur de solutions Microsoft Cloud jusqu’au 31 janvier 2020. Pour plus d’informations sur la chronologie, consultez le tableau suivant :

| Date | Jalon | Détails |
|------------|------------|--------------------------------|
|1er août 2019|Aperçu de l’expérience utilisateur disponible dans le bac à sable|Les partenaires peuvent confirmer l’acceptation par le client du contrat client Microsoft à l’aide du tableau de bord de l’Espace partenaires dans l’environnement du bac à sable (sandbox) CSP. Les partenaires ayant accès à l’environnement du bac à sable (sandbox) CSP peuvent afficher un aperçu des modifications de l’expérience utilisateur. Les partenaires sans accès au bac à sable peuvent en savoir plus sur les modifications apportées dans cette rubrique.|
|3 septembre 2019|L’aperçu de l’API est disponible dans le bac à sable.|Le partenaire peut confirmer l’acceptation par le client du contrat client Microsoft à l’aide du l’API de l’Espace partenaires dans l’environnement du bac à sable (sandbox) CSP. Les partenaires de l’API peuvent utiliser cette opportunité pour afficher un aperçu des modifications de l’API et commencer à travailler sur l’intégration de l’API pour prendre en charge le nouveau contrat.|
|20 septembre, 2019|Le kit de développement logiciel (SDK) .NET (préversion) est disponible dans le bac à sable.|Le partenaire peut confirmer l’acceptation par le client du Contrat client Microsoft à l’aide du SDK .NET de l'Espace partenaires dans l’environnement de bac à sable Fournisseur de solutions Microsoft Cloud. Les partenaires de l’API peuvent utiliser cette opportunité pour afficher un aperçu des modifications du kit de développement logiciel (SDK) .NET et commencer à travailler sur l’intégration de l’API pour prendre en charge le nouveau contrat.|
|1er octobre 2019|Contrat client Microsoft disponible en production|Microsoft présente le contrat client Microsoft au programme CSP pour remplacer le contrat Microsoft Cloud. Les partenaires peuvent confirmer l’acceptation par le client du contrat client Microsoft à l’aide de l’API et du tableau de bord de l’Espace partenaires en production. Le contrat Microsoft Cloud reste pris en charge dans le programme partenaire CSP. Toutefois, les partenaires sont invités à commencer à migrer vers le contrat client Microsoft. Les nouveaux achats et les modifications apportées au nombre de sièges dans les abonnements existants nécessitent la confirmation par le partenaire du contrat client Microsoft ou du contrat Microsoft Cloud. Certaines nouvelles offres (par exemple, le nouveau plan Azure) requièrent la confirmation du contrat client Microsoft.|
|31 janvier 2020|Contrat Microsoft Cloud supprimé de la production|Le contrat Microsoft Cloud n’est plus accepté dans le programme partenaire CSP. Les nouveaux achats et les modifications apportées au nombre de sièges dans les abonnements existants nécessitent la confirmation par le partenaire du contrat client Microsoft. Cette exigence s’applique aux nouveaux clients et aux clients existants qui ont peut-être déjà accepté le contrat Microsoft Cloud.|

## <a name="access-microsoft-customer-agreement-template"></a>Accéder au modèle de contrat client Microsoft
Les partenaires peuvent télécharger manuellement la dernière version du modèle de contrat client Microsoft à partir d' [ici](https://aka.ms/customeragreement). Notez que le contrat client Microsoft est spécifique au pays. Lorsque vous demandez le modèle de contrat client Microsoft, veillez à sélectionner le pays approprié en fonction de l’emplacement du client. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmer l’acceptation du client à l’aide de l’API espace partenaires/SDK
Les partenaires peuvent utiliser l’API/le kit de développement logiciel (SDK) de l’espace partenaires pour confirmer l’acceptation du client par le contrat client Microsoft. Pour plus d’informations sur l’API/le kit de développement logiciel (SDK), consultez :

- [Obtenir les métadonnées du Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confirmer l'acceptation par le client du Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtenir une confirmation de l'acceptation par le client du Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtenir un lien de téléchargement pour le modèle de Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>Confirmer l’acceptation du client dans l'Espace partenaires
Les partenaires peuvent confirmer l’acceptation par le client de l’accord de client Microsoft dans l’espace partenaires pour les nouveaux clients et les clients existants.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmer l’acceptation par les nouveaux clients

Lorsque vous créez un locataire client dans l’Espace partenaires, suivez les étapes ci-dessous pour confirmer l’acceptation par le client du contrat client Microsoft. Vous devez être Agent administrateur ou Commercial pour suivre ces étapes.

1. Sélectionnez **Clients**, puis **Nouveau client**.

2. Sous **Informations sur le compte**, entrez les informations relatives à l’entreprise et à son contact principal.

3. Sous **Contrat Microsoft**, sélectionnez le **Contrat client Microsoft**.

4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Assurez-vous que les coordonnées de l’utilisateur principal affichées sont correctes. Si elles ne sont pas correctes, sélectionnez **Mettre à jour**, puis saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.

![Nouveau client](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmer l’acceptation par les clients existants

Vous devez être Agent administrateur ou Commercial pour effectuer cette opération :

1. Sélectionnez **Clients**. Recherchez et sélectionnez le client.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.

4. Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Sélectionnez **Enregistrer** et continuez.

![Client existant](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Récupérer la confirmation de l’acceptation par le client

Vous pouvez récupérer la confirmation qu’un client existant a accepté le contrat client Microsoft en suivant les étapes ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, vérifiez si la confirmation a été fournie ou n’a pas été fournie par ce client.
