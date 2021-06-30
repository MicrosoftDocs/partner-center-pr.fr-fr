---
title: Enregistrer vos transactions
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lorsque vous inscrivez un contrat que vous avez remporté dans l’espace partenaires, Microsoft vous offre plus d’opportunités à l’avenir.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080659"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Inscrire les demandes que vous avez remportées dans l’espace partenaires

**Rôles appropriés** : Administrateur des références

Vous pouvez enregistrer les transactions que vous avez conclues dans l’Espace partenaires en fournissant des informations supplémentaires sur le contrat. Ces informations nous permettent de vous proposer ensuite plus d’opportunités.

Il existe deux chemins d’accès qui mènent à l’enregistrement des transactions :

- Vous avez créé un nouveau contrat dans la section **opportunités de covente** , et votre transaction répond aux critères d’enregistrement des transactions.
- Vous souhaitez signaler une transaction ISV Connect fermée, qui n’a pas été co-vendue avec Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Inscrire une transaction provenant d’une opportunité de covente

Si vous envisagez d’inscrire une transaction provenant d’une opportunité de covente, votre offre doit répondre aux conditions d’éligibilité suivantes :

- Le type de contrat est « covente » ou « partenaire » (vous avez choisi d’autoriser les vendeurs Microsoft à consulter cette offre).
- Il existe au moins une solution éligible dans le contrat. Une solution est éligible si elle contient au moins l’une des balises suivantes :
  - Co-vente Azure IP
  - Business Applications Premium
  - Business Applications standard
- L’état de la transaction est « gagné ».
- Si le type de contrat est covente, Microsoft doit avoir accepté l’invitation ou marqué le contrat comme conclu. Vous pouvez voir l’état Microsoft en regardant la carte Microsoft sous les détails de votre contrat.

Si vous avez respecté les conditions d’éligibilité, vous êtes automatiquement invité à inscrire votre demande avec un bouton **s’inscrire maintenant** sur la barre de progression des transactions :

:::image type="content" source="images/register-deals.png" alt-text="Capture d’écran montrant la barre de progression des transactions.":::

> [!NOTE]
> Si l’élément **d’enregistrement** de la transaction ne s’affiche pas dans la barre de progression des transactions pour votre transaction, le contrat ne répond pas à toutes les conditions requises pour l’enregistrement des transactions.

Une fois que vous avez cliqué sur **inscrire**, vous êtes redirigé vers la page d’enregistrement de la demande et vous êtes invité à remplir un formulaire contenant des informations préremplies pour votre client et votre solution. Remplissez le formulaire à l’aide des instructions ci-dessous, puis cliquez sur **inscrire**.

Lors de l’inscription, un ou deux enregistrements d’enregistrement des transactions seront créés en fonction de la solution.

- Si votre solution est éligible pour la connexion ISV, un enregistrement d’inscription de la transaction ISV Connect sera créé. Cet enregistrement d’enregistrement de transaction sera utilisé pour la facturation.
- Si votre solution est éligible à des incentives de covente IP, un enregistrement d’inscription de vente de covente IP est créé. Cet enregistrement d’enregistrement de transaction sera revu et approuvé ou rejeté par l’équipe de révision des ventes de covente.

## <a name="report-a-closed-isv-connect-deal"></a>Signaler une transaction de connexion ISV fermée

Pour signaler une transaction ISV Connect fermée, accédez à l’onglet **d’enregistrement des transactions** , puis cliquez sur **+ signaler la transaction connexion ISV fermée**. Renseignez les champs requis, puis cliquez sur **inscrire**. Cet enregistrement d’enregistrement de transaction sera utilisé pour la facturation.

## <a name="fill-out-the-deal-registration-form"></a>Remplissez le formulaire d’enregistrement des transactions

> [!NOTE]
> Vous pouvez filtrer les demandes par nom de client, État et type de contrat. Pour ce faire, cliquez sur le bouton **filtre** en haut de la page d’enregistrement des transactions.

Que vous ayez affaire à l’inscription d’une opportunité de covente ou que vous signaliez une transaction ISV Connect fermée, qui n’a pas été commercialisée avec Microsoft, vous serez invité à renseigner les champs suivants sur le formulaire d’inscription aux ventes.

- **Détails du client**: entrez le nom de la **société** de votre client et sélectionnez son **pays/région**. Entrez ensuite sa **Ville** et son **État/Province**.
- **Solution**: sélectionnez la solution qui sera utilisée pour la transaction. Si la solution appropriée ne s'affiche pas, contactez le support.
- **Type de contrat**: indiquez si cette transaction est un **nouveau** contrat ou un **renouvellement** d’un contrat précédent.
- **Valeur totale du contrat**: valeur totale attendue pour l’engagement. Cette valeur doit inclure tous les frais liés aux logiciels et aux services, mais pas les coûts matériels. Veillez à sélectionner la devise qui convient.
- **Valeur** de la solution : valeur totale de la solution cloud qui sera utilisée pour la transaction. Veillez à inclure tous les coûts associés aux frais liés aux logiciels et à la maintenance, mais n’incluez pas les éléments remboursables, les frais de personnalisation non périodiques ou les frais de licence Fournisseur de solutions Microsoft Cloud directement associés payés par Microsoft.
- **La solution sera-t-elle déployée sur Azure ? Si ce n’est pas le cas, choisissez autre**: **Azure** ou **autre**.
- **La consommation de la solution s’exécutera-t-elle sur le locataire partenaire ou le locataire client ?**: sélectionnez le locataire **client** ou le **locataire partenaire**.
- **Date de début du contrat**: date de début du contrat. Pour les offres de paiement à l’utilisation (PAYG), utilisez la date de la première facture. Par défaut, l’espace partenaires ne vous permet pas d’entrer une date de début antérieure à la date de signature du contrat. Cela peut avoir un impact sur certaines transactions, telles que les déploiements d’IP qui commencent avant la date de signature. Pour pouvoir entrer ces demandes, utilisez la date de signature du contrat pour **les** champs date de signature et date de début lorsque vous envoyez. (Le contrat doit indiquer explicitement la durée de la transaction pour que ACV puisse être calculé correctement.)
- **Date de fin du contrat**: si le contrat se termine à une date spécifique, sélectionnez **a une date de fin** et indiquez cette date. Si le contrat n’a pas de date de fin spécifique, sélectionnez **perpétuelle**. Pour les offres de paiement à l’utilisation (PAYG), utilisez la date de la dernière facture ou la plus récente.
- **Date de signature du contrat**: date à laquelle le contrat final a été signé par votre organisation et par le client. Pour les offres de paiement à l’utilisation (PAYG), utilisez la date de la première facture.
- **Contact d’inscription**: le **prénom**, le **nom**, le **numéro de téléphone** et l’adresse de **messagerie** d’une personne de votre organisation que nous pouvons contacter si nous avons besoin de plus de détails sur les informations fournies ici.

Lorsque vous avez terminé toutes les sections de la page, cliquez sur **inscrire**.

- Si la transaction est une transaction ISV Connect, vous remarquerez que l’état de la transaction est « sent, Completed ». Aucune autre action n’est requise sur cet enregistrement d’enregistrement de transaction. Cet enregistrement sera utilisé pour la facturation.
- Si le contrat est un contrat de covente IP, vous remarquerez que l’état de la transaction est « soumis ». L’équipe de révision des transactions de covente Microsoft passera en revue les informations que vous avez fournies dans cet enregistrement d’inscription. L’équipe de révision demandera plus d’action si nécessaire, ou l’approuvera ou la rejettera directement.
- Si vous enregistrez une transaction provenant d’une opportunité de covente, et que vous constatez que deux enregistrements d’enregistrement de transaction ont été créés, cela signifie que la solution sur votre vente est éligible pour la connexion ISV et pour la covente IP. L’enregistrement ISV Connect sera utilisé pour la facturation. L’enregistrement de covente IP est examiné par l’équipe de validation de la vente par covente.

