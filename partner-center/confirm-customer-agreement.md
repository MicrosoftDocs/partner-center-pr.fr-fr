---
title: Comment vérifier que votre client a accepté le Contrat client Microsoft pour le programme Fournisseur de solutions Microsoft Cloud
description: Les partenaires fournisseurs de solutions Cloud (CSP) doivent confirmer l’acceptation par le client du Contrat client Microsoft avant de leur commander des services Microsoft.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633776"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Comment vérifier que votre client a accepté le Contrat client Microsoft pour le programme Fournisseur de solutions Microsoft Cloud

**Rôles appropriés**

- Agent d’administration
- Agent commercial


Les clients disposent de deux options pour accepter le Contrat client Microsoft.

**Option 1** : Attestation du partenaire de l’acceptation par les clients - Le partenaire peut confirmer l’acceptation par les clients à l’aide de l’API/du kit SDK de l’Espace partenaires ou via le tableau de bord de l’Espace partenaires.

**Option 2** : Acceptation directe par le client - Le partenaire peut inviter le client via une URL à passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Accéder au modèle de Contrat client Microsoft

Vous pouvez télécharger manuellement la dernière version du modèle de Contrat client Microsoft à partir d’[ici](https://aka.ms/customeragreement). Le Contrat client Microsoft est spécifique au pays. Quand vous demandez le modèle de Contrat client Microsoft, veillez à sélectionner le pays approprié en fonction de la localisation du client.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Option 1 : Confirmer l’acceptation du client dans l'Espace partenaires

Les partenaires de facturation directe peuvent confirmer l’acceptation par les clients du Contrat client Microsoft dans l’Espace partenaires pour les clients nouveaux et existants. Les revendeurs indirects ne peuvent pas effectuer d’attestation au nom de leurs clients. Ils doivent collaborer avec leur fournisseur indirect pour obtenir l’attestation.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmer l’acceptation par les nouveaux clients

Lorsque vous créez un locataire client dans l’Espace partenaires, suivez les étapes ci-dessous pour confirmer l’acceptation par le client du contrat client Microsoft. Vous devez être Agent administrateur ou Commercial pour suivre ces étapes.

1. Sélectionnez **Clients**, puis **Nouveau client**.

2. Sous **Informations sur le compte**, entrez les informations relatives à l’entreprise et à son contact principal.

3. Sous **Contrat Microsoft**, cochez la case permettant d’attester que le client a accepté le Contrat client Microsoft.

4. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Assurez-vous que les coordonnées de l’utilisateur principal affichées sont correctes. Si ce n’est pas le cas, sélectionnez **Mettre à jour** et entrez les informations exactes de la personne qui a accepté le contrat.

6. Sélectionnez **Suivant** pour continuer à créer le locataire du client.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nouveau client":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmer l’acceptation par les clients existants

Pour ce faire, vous devez être un agent d’administration ou un commercial :

1. Sélectionnez **Clients**. Recherchez et sélectionnez le client.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.

4. Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

5. Sélectionnez **Enregistrer** et continuez.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Client existant":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Récupérer la confirmation de l’acceptation par le client

Pour récupérer la confirmation qu’un client existant a accepté le Contrat client Microsoft, procédez comme suit. Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.

1. Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.

2. Sélectionnez **Informations sur le compte**.

3. Sous **Contrat client Microsoft**, vérifiez si la confirmation a été fournie ou n’a pas été fournie par ce client.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmer l’acceptation par les clients à l’aide de l’API/du kit SDK de l’Espace partenaires

Vous pouvez utiliser l’API/le kit SDK de l’Espace partenaires pour confirmer l’acceptation du Contrat client Microsoft par les clients. Pour plus d’informations sur l’API/le SDK, consultez :

- [Obtenir les métadonnées du Contrat client Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Confirmer que le client a accepté le Contrat client Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtenir la confirmation de l’acceptation du Contrat client Microsoft par le client](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtenir un lien de téléchargement pour le modèle de Contrat client Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Option 2 : Acceptation par les clients dans le Centre d’administration Microsoft 365

Les partenaires peuvent inviter de nouveaux clients et des clients existants, via une URL, à passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365. Les sections suivantes vous montrent comment :

- Créer un client, puis l’inviter à passer en revue et accepter le contrat.

- Inviter un nouveau client à passer en revue et accepter la relation de revendeur et le contrat.

- Inviter un client existant à passer en revue et accepter le contrat.

>[!NOTE]
> Vous pouvez utiliser l’[API ou le SDK de l’Espace partenaires](/partner-center/develop/get-direct-sign-status-of-customer-agreement) pour savoir si le client a accepté directement le Contrat client Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Créer un client, puis l’inviter à passer en revue et accepter le contrat

Effectuez les étapes suivantes pour créer un client dans l’Espace partenaires, puis invitez-le à passer en revue et accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365.

1. Sous l’onglet **Clients** de l’Espace partenaires, sélectionnez **Ajouter un client**.

2. Sous **Informations sur le compte**, entrez les informations relatives au nouveau client dans tous les champs obligatoires, notamment le nom de l’entreprise et le contact principal du client.

3. Sous **Contrat client**, sélectionnez **Le client va être invité à accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365**. Remplissez tous les autres champs obligatoires de la page.

4. Sélectionnez **Suivant : Passer en revue**, puis poursuivez les étapes permettant de créer le locataire du client. 

>[!NOTE] 
>Les nouveaux clients ne peuvent pas effectuer d’achat tant qu’ils n’ont pas accepté le Contrat client Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Créer un client":::

5. Une fois que vous avez atteint l’écran **Confirmation** dans le workflow de nouveau client, enregistrez les informations d’identification de ce client. Vous devrez plus tard fournir ces informations d’identification à votre client.

6. En dehors de l’Espace partenaires, créez et envoyez un e-mail invitant le client à accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365. Veillez à inclure ces éléments dans l’e-mail :

   - Lien vers cette [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (connexion obligatoire)

   - Informations d’identification du client, que vous avez enregistrées à l’étape 5.

7. Le client va ensuite recevoir l’invitation par e-mail de la part du partenaire et sélectionner l’[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Le client se connecte au Centre d’administration Microsoft 365 à l’aide des informations d’identification que vous avez fournies.

9. Le client coche la case pour accepter le Contrat client Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Inviter un nouveau client à passer en revue et accepter la relation de revendeur et le Contrat client Microsoft 

Effectuez les étapes suivantes pour inviter un nouveau client à passer en revue et accepter la relation de revendeur et le Contrat client Microsoft. 

1. Sous l’onglet **Clients** de l’Espace partenaires, sélectionnez le lien **Demander une relation de revendeur**. 

2. Un modèle d’e-mail automatique est généré. Il comprend notamment du texte et une URL paramétrable qui dirige le client vers le Centre d’administration Microsoft 365.

3. Vous pouvez personnaliser le modèle d’e-mail généré automatiquement, puis sélectionner **Copier dans le Presse-papiers** ou **Ouvrir un e-mail**.

4. Utilisez ce modèle d’e-mail pour inviter le client à accepter la **demande de relation de revendeur** et le **Contrat client Microsoft**. (Remarque : Dans l’invitation par e-mail, vérifiez que le partenaire ajoute également l’URL fournie automatiquement ainsi que les informations d’identification client créées.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="créer une relation":::

5. Le client reçoit une invitation par e-mail, et clique sur l’URL paramétrable. 

6. Le client utilise les informations d’identification que vous avez fournies dans l’e-mail pour se connecter au Centre d’administration Microsoft 365.

7. Le client coche la case pour accepter la **relation de revendeur** et le **Contrat client Microsoft**. 

8. Dans la même URL, le client peut voir une liste centralisée des différents partenaires avec lesquels il travaille. Il peut sélectionner un partenaire pour voir les détails correspondants.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Accepter le contrat":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Inviter un client existant à passer en revue et accepter le contrat

Effectuez les étapes suivantes pour inviter un client existant à passer en revue et accepter le Contrat client Microsoft. 

1. Créez l’e-mail destiné au client avec l’URL intégrée invitant le client à accepter le Contrat client Microsoft.

2. Votre client reçoit l’invitation par e-mail, puis clique sur l’[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Le client entre ses informations d’identification dans le Centre d’administration Microsoft 365.

4. Votre client coche la case pour accepter le Contrat client Microsoft. 

5. Dans la même URL, le client peut voir la liste centralisée des différents partenaires avec lesquels il travaille. Il peut sélectionner un partenaire pour voir les détails correspondants.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="client":::

>[!NOTE]
>Dans certains scénarios, les clients ne peuvent pas toujours accepter directement le Contrat client Microsoft. Pour en savoir plus sur ces situations, consultez ci-après Deux scénarios où vous devez effectuer l’attestation au nom de votre client.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Deux scénarios où vous devez effectuer l’attestation au nom de votre client

Il existe deux scénarios où les clients ne peuvent pas toujours accepter directement le Contrat client Microsoft dans le Centre d’administration Microsoft 365.

**Scénario 1** : Un client existant a acheté l’un des produits suivants via une relation partenaire existante : offres, logiciels ou abonnements logiciels, instances réservées ou plan Azure. Le client tente à présent d’effectuer un nouvel achat (en dehors du renouvellement automatique). Quand ce client clique sur l’URL, il reçoit un message de ce type : « Contactez votre partenaire pour confirmer votre acceptation du Contrat client Microsoft ».  

**Solution** : Vous devez effectuer l’attestation au nom du client.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Capture d’écran de la page du Centre d’administration Microsoft 365 vous invitant à contacter votre partenaire pour confirmer l’acceptation du Contrat client Microsoft.":::

**Scénario 2** : Un client existant a acheté des offres, des logiciels ou des abonnements logiciels, des instances réservées ou un plan Azure. Le client tente à présent d’effectuer un nouvel achat auprès d’un nouveau partenaire.

Quand le client clique sur l’URL du Centre d’administration Microsoft 365 pour accepter la nouvelle relation partenaire et le contrat, il reçoit un message de ce type : « Contactez votre partenaire pour confirmer votre acceptation du Contrat client Microsoft ».  

**Solution** : Vous devez effectuer l’attestation au nom du client.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Confirmer qu’un client a accepté le contrat

Si vous essayez de créer une commande pour un client existant que vous n’avez pas encore confirmé, vous recevrez une invite pour effectuer la confirmation. Pour ce faire, utilisez la procédure suivante.

1. Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.

2. Sous **Date d'acceptation du contrat**, entrez la date appropriée. Vous ne pouvez pas la définir sur une date ultérieure.

3. Sélectionnez **Enregistrer et continuer**. 

## <a name="next-steps"></a>Étapes suivantes

- [Vérifier ou mettre à jour les informations du profil de votre entreprise](update-your-partner-profile.md)
- [Contrats client Microsoft (par région, par langue)](Agreements.md)
