---
title: Confirmer l’acceptation du Contrat client Microsoft par les clients
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment confirmer l’acceptation du Contrat client Microsoft par les clients. Les fournisseurs de solutions Cloud doivent faire cela pour commander des produits et services Microsoft pour les clients.
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, MCA, Contrat Microsoft Cloud, Contrat client Microsoft, modèles de contrat client
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ae3605f0cb352b6efb18c7e53d9842d35c7e00c3
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908165"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Confirmer l’acceptation du Contrat client Microsoft par le client dans le cadre du programme des partenaires fournisseurs de solutions Cloud

**S’applique à**

- Espace partenaires
- Centre d’administration Microsoft 365

**Rôles appropriés**

- Agent d’administration
- Agent commercial

**Types de partenaire appropriés**

- Revendeurs indirects, partenaires effectuant une facturation directe, fournisseurs indirects


Le 1er octobre 2019, Microsoft a introduit le **Contrat client Microsoft** dans le programme Fournisseur de solutions Cloud pour remplacer le contrat Microsoft Cloud. Lisez l’[aide](indirect-reseller-tasks-in-partner-center.md) supplémentaire destinée aux revendeurs indirects. Pour faciliter la migration des partenaires vers le nouveau contrat, les deux contrats ont coexisté dans le programme CSP jusqu’au 31 janvier 2020. Depuis le 1er février 2020, le contrat client Microsoft a remplacé le contrat Microsoft Cloud.

Les clients disposent de deux options pour accepter le Contrat client Microsoft. 

**Option 1** : Attestation du partenaire de l’acceptation par les clients - Le partenaire peut confirmer l’acceptation par les clients à l’aide de l’API/du kit SDK de l’Espace partenaires ou via le tableau de bord de l’Espace partenaires.

**Option 2** : Acceptation directe par le client - Le partenaire peut inviter le client via une URL à passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Accéder au modèle de Contrat client Microsoft

Vous pouvez télécharger manuellement la dernière version du modèle de Contrat client Microsoft à partir d’[ici](https://aka.ms/customeragreement). Le Contrat client Microsoft est spécifique au pays. Quand vous demandez le modèle de Contrat client Microsoft, veillez à sélectionner le pays approprié en fonction de la localisation du client. 

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Option 1 : Confirmer l’acceptation du client dans l'Espace partenaires

Les partenaires peuvent confirmer l’acceptation par les clients du Contrat client Microsoft dans l’Espace partenaires pour les clients nouveaux et existants. Les revendeurs ne peuvent pas effectuer d’attestation au nom de leurs clients. Ils doivent collaborer avec leur fournisseur indirect pour obtenir l’attestation.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmer l’acceptation par les nouveaux clients

Lorsque vous créez un locataire client dans l’Espace partenaires, suivez les étapes ci-dessous pour confirmer l’acceptation par le client du contrat client Microsoft. Vous devez être Agent administrateur ou Commercial pour suivre ces étapes.

1. Sélectionnez **Clients**, puis **Nouveau client**.

2. Sous **Informations sur le compte**, entrez les informations relatives à l’entreprise et à son contact principal.

3. Sous **Contrat Microsoft**, cochez la case permettant d’attester que le client a accepté le Contrat client Microsoft. 

4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Assurez-vous que les coordonnées de l’utilisateur principal affichées sont correctes. Si ce n’est pas le cas, sélectionnez **Mettre à jour** et entrez les informations exactes de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour continuer à créer le locataire du client.

![Nouveau client](images/mca/newcustomeragreement.jpg)  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmer l’acceptation par les clients existants

Pour ce faire, vous devez être un agent d’administration ou un commercial :

1. Sélectionnez **Clients**. Recherchez et sélectionnez le client.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.

4. Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Sélectionnez **Enregistrer** et continuez.

![Client existant](images/mcua2-update2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Récupérer la confirmation de l’acceptation par le client

Vous pouvez récupérer la confirmation qu’un client existant a accepté le contrat client Microsoft en suivant les étapes ci-dessous. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, vérifiez si la confirmation a été fournie ou n’a pas été fournie par ce client.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmer l’acceptation par les clients à l’aide de l’API/du kit SDK de l’Espace partenaires

Vous pouvez utiliser l’API/le kit SDK de l’Espace partenaires pour confirmer l’acceptation du Contrat client Microsoft par les clients. Pour plus d’informations sur l’API/le SDK, consultez :

- [Obtenir les métadonnées du Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confirmer l'acceptation par le client du Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtenir une confirmation de l'acceptation par le client du Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtenir un lien de téléchargement pour le modèle de Contrat client Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Option 2 : Acceptation par les clients dans le Centre d’administration Microsoft 365

Les partenaires peuvent inviter de nouveaux clients et des clients existants, via une URL, à passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365. Les sections suivantes vous montrent comment :

- Créer un client, puis l’inviter à passer en revue et accepter le contrat.

- Inviter un nouveau client à passer en revue et accepter la relation de revendeur et le contrat.

- Inviter un client existant à passer en revue et accepter le contrat.

>[!NOTE]
> Vous pouvez utiliser l’[API ou le SDK de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) pour savoir si le client a accepté directement le Contrat client Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Créer un client, puis l’inviter à passer en revue et accepter le contrat

Effectuez les étapes suivantes pour créer un client dans l’Espace partenaires, puis invitez-le à passer en revue et accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365.

1. Sous l’onglet **Clients** de l’Espace partenaires, sélectionnez **Ajouter un client**.

2. Sous **Informations sur le compte**, entrez les informations relatives au nouveau client dans tous les champs obligatoires, notamment le nom de l’entreprise et le contact principal du client.

3. Sous **Contrat client**, sélectionnez la première option, **Le client va être invité à accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365**. Remplissez tous les autres champs obligatoires de la page.

4. Sélectionnez **Suivant : Passer en revue**, puis poursuivez les étapes permettant de créer le locataire du client. (Remarque : Les nouveaux clients ne peuvent pas effectuer de nouvel achat tant qu’ils n’ont pas accepté le Contrat client Microsoft.)  

![Créer un client](images/mca/create-new-customer.jpg)

5. Une fois que vous avez atteint l’écran **Confirmation** dans le workflow de nouveau client, enregistrez les informations d’identification de ce client. Vous devrez plus tard fournir ces informations d’identification à votre client.

6. En dehors de l’Espace partenaires, créez et envoyez un e-mail invitant le client à accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365. Veillez à inclure ces éléments dans l’e-mail :

   - Lien vers cette [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (connexion obligatoire)

   - Informations d’identification du client, que vous avez enregistrées à l’étape 5.

7. Le client va ensuite recevoir l’invitation par e-mail de la part du partenaire et sélectionner l’[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Le client se connecte au Centre d’administration Microsoft 365 à l’aide des informations d’identification reçues de la part du partenaire.

9. Le client coche ensuite la case pour accepter le Contrat client Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Inviter un nouveau client à passer en revue et accepter la relation de revendeur et le Contrat client Microsoft 

Effectuez les étapes suivantes pour inviter un nouveau client à passer en revue et accepter la relation de revendeur et le Contrat client Microsoft. 

1. Sous l’onglet **Clients** de l’Espace partenaires, sélectionnez le lien **Demander une relation de revendeur**. 

2. Un modèle d’e-mail automatique est généré. Il comprend notamment du texte et une URL paramétrable pour diriger le client vers le Centre d’administration Microsoft 365.

3. Vous pouvez personnaliser le modèle d’e-mail généré automatiquement, puis sélectionner **Copier dans le Presse-papiers** ou **Ouvrir un e-mail**.

4. Utilisez ce modèle d’e-mail pour inviter le client à accepter la **demande de relation de revendeur** et le **Contrat client Microsoft**. (Remarque : Dans l’invitation par e-mail, vérifiez que le partenaire ajoute également l’URL fournie automatiquement ainsi que les informations d’identification client créées.)

![créer une relation](images/mca/createrelationship.png)

5. Le client reçoit une invitation par e-mail, et clique sur l’URL paramétrable. 

6. Le client utilise les informations d’identification fournies par le partenaire dans l’e-mail pour se connecter au Centre d’administration Microsoft 365.

7. Le client coche la case pour accepter la **relation de revendeur** et le **Contrat client Microsoft**. 

8. Dans la même URL, le client peut voir une liste centralisée des différents partenaires avec lesquels il travaille. Il peut sélectionner un partenaire pour voir les détails correspondants.

![Accepter le contrat](images/mca/accept.jpg)


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Inviter un client existant à passer en revue et accepter le contrat 

Effectuez les étapes suivantes pour inviter un client existant à passer en revue et accepter le Contrat client Microsoft. 

1. Créez l’e-mail destiné au client avec l’URL intégrée invitant le client à accepter le Contrat client Microsoft.

2. Votre client reçoit l’invitation par e-mail, puis clique sur l’[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Le client entre ses informations d’identification dans le Centre d’administration Microsoft 365.

4. Votre client coche la case pour accepter le Contrat client Microsoft. 

5. Dans la même URL, le client peut voir la liste centralisée des différents partenaires avec lesquels il travaille. Il peut sélectionner un partenaire pour voir les détails correspondants.

![client](images/mca/customeraccept.png)

>[!NOTE]
>Dans certains scénarios, les clients ne peuvent pas toujours accepter directement le Contrat client Microsoft. Pour en savoir plus sur ces situations, consultez [Deux scénarios où vous devez effectuer l’attestation au nom de votre client](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Détails de la chronologie de l’historique

| Date | Jalon | Détails |
|------------|------------|--------------------------------|
|1er août 2019|Aperçu de l’expérience utilisateur disponible dans le bac à sable|Les partenaires peuvent confirmer l’acceptation par le client du contrat client Microsoft à l’aide du tableau de bord de l’Espace partenaires dans l’environnement du bac à sable (sandbox) CSP. Les partenaires ayant accès à l’environnement du bac à sable (sandbox) CSP peuvent afficher un aperçu des modifications de l’expérience utilisateur. Les partenaires sans accès au bac à sable peuvent en savoir plus sur les modifications apportées dans cette rubrique.|
|3 septembre 2019|L’aperçu de l’API est disponible dans le bac à sable.|Le partenaire peut confirmer l’acceptation par le client du contrat client Microsoft à l’aide du l’API de l’Espace partenaires dans l’environnement du bac à sable (sandbox) CSP. Les partenaires de l’API peuvent utiliser cette opportunité pour afficher un aperçu des modifications de l’API et commencer à travailler sur l’intégration de l’API pour prendre en charge le nouveau contrat.|
|20 septembre 2019|Le kit de développement logiciel (SDK) .NET (préversion) est disponible dans le bac à sable.|Le partenaire peut confirmer l’acceptation par le client du Contrat client Microsoft à l’aide du SDK .NET de l'Espace partenaires dans l’environnement de bac à sable Fournisseur de solutions Microsoft Cloud. Les partenaires de l’API peuvent utiliser cette opportunité pour afficher un aperçu des modifications du kit de développement logiciel (SDK) .NET et commencer à travailler sur l’intégration de l’API pour prendre en charge le nouveau contrat.|
|1er octobre 2019|Contrat client Microsoft disponible en production|Microsoft présente le contrat client Microsoft au programme CSP pour remplacer le contrat Microsoft Cloud. Les partenaires peuvent confirmer l’acceptation par le client du contrat client Microsoft à l’aide de l’API et du tableau de bord de l’Espace partenaires en production. Le contrat Microsoft Cloud reste pris en charge dans le programme partenaire CSP. Toutefois, les partenaires sont invités à commencer à migrer vers le contrat client Microsoft. Les nouveaux achats et les modifications apportées au nombre de sièges dans les abonnements existants nécessitent la confirmation par le partenaire du contrat client Microsoft ou du contrat Microsoft Cloud. Certaines nouvelles offres (par exemple, le nouveau plan Azure) requièrent la confirmation du contrat client Microsoft.|
|31 janvier 2020|Contrat Microsoft Cloud supprimé de la production|Le contrat Microsoft Cloud n’est plus accepté dans le programme partenaire CSP. Les nouveaux achats et les modifications apportées au nombre de sièges dans les abonnements existants nécessitent la confirmation par le partenaire du contrat client Microsoft. Cette exigence s’applique aux nouveaux clients et aux clients existants qui ont peut-être déjà accepté le contrat Microsoft Cloud.|
|3 février 2020|Le partenaire peut désormais inviter le client via une URL pour passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365 authentifié. | Le client peut accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365. L’acceptation directe par le client du contrat dans le Centre d’administration Microsoft 365 confirme l’approbation des conditions. 
