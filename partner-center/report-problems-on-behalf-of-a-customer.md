---
title: Signaler des problèmes au nom d’un client
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment faire remonter un problème de service client à Microsoft et comment transmettre un ticket de support pour les différents types de services Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80c617a97575fea3003ea8652d48396412033cc7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441946"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Signaler un problème de service au nom d’un client, y compris quand et comment procéder

**S’applique à**

- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Fournisseurs indirects

Si votre client rencontre un problème de service que vous ne pouvez pas résoudre et que celui-ci répond aux critères décrits dans [escalader les problèmes à Microsoft](escalate-problems-to-microsoft.md), votre fournisseur indirect peut créer un ticket de support pour eux. Ce processus est également utile pour faire remonter des problèmes ou des litiges de facturation, ou en cas de fraudes.

## <a name="submit-a-service-request-for-a-customer"></a>Envoyer une demande de service pour un client

1. Dans le menu de l’espace partenaires, sous CSP, sélectionnez **clients** .

2. Sur la page clients, sélectionnez ou recherchez le client de votre choix
    
3. Dans le menu client, sélectionnez **demandes de service** .

4. À partir du menu déroulant **Nouvelle demande**, sélectionnez **Azure** ou **Office 365, Dynamics 365, Enterprise Mobility Suite**. Vous êtes redirigé vers le Portail Microsoft Azure ou le centre d’administration Office 365.

>[!NOTE]
>Les partenaires d’opérations de support transmettant Dynamics 365 dans CSP sont tenus de conserver un contrat de support pour le plan ASfP (Advanced support for Partner) ou une version ultérieure. Ce contrat de support est nécessaire pour envoyer des incidents Dynamics 365 pour le compte d’un client CSP. [En savoir plus](https://partner.microsoft.com/support/partnersupport) sur les options du contrat de support.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Lorsque vous avez besoin de créer une demande de service pour votre client dans Azure, tenez compte des éléments suivants :
>
>- Pour que vous, en tant que revendeur indirect, vous puissiez créer des demandes de service pour votre client dans Azure, votre fournisseur indirect doit vous accorder l’accès au compte Azure du client. Cela diffère de l'administration pour le compte des clients pour Office 365.
>
>- Même si l’administrateur du support technique de l’Espace partenaires ne peut pas créer de demandes de service dans le portail des services Azure, il peut créer un groupe de support dans le portail des services Azure et autoriser ce groupe à consigner des demandes de support.

1. Sélectionnez **Nouvelle demande de support**.

2. Remplissez la demande de support à l’aide des informations appropriées, puis sélectionnez **Créer**&nbsp;:

   - Dans la section **Notions de base** de la demande de support, veillez à sélectionner **Fournisseur de solutions Cloud** dans le champ **Formule d’assistance**.

   - Dans la section **Coordonnées** de la demande de support, entrez vos coordonnées, pas celles de votre client.

3. Passez en revue ultérieurement les demandes de service de votre client dans le portail Microsoft Azure en sélectionnant **Gérer les demandes de support**.

Vous devrez peut-être créer une demande de support pour un client lorsque vous n’avez pas les autorisations d’administrateur pour ce client. Cela peut se produire dans deux cas :

- Vous n’avez pas demandé de privilèges d’administrateur lorsque vous avez établi la relation pour la première fois.
- Vous gérez uniquement les abonnements Azure d’un client, de sorte que vous n’avez pas d’autorisations d’administration.
 
Dans l’un ou l’autre de ces cas, vous pouvez utiliser la procédure suivante pour créer une demande de support. 

1. Copiez le nom de domaine du client à partir de la page de son compte dans l’espace partenaires.

2. Accédez à https://portal.azure.com/[customerdomainname]. 

3. Sélectionnez l’abonnement Azure qui requiert le support.

4. Sélectionnez **Nouvelle demande de support**, puis suivez les invites pour créer la demande. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office&nbsp;365, Microsoft Dynamics&nbsp;CRM Online, Enterprise Mobility Suite

1. Dans la section **créer une demande de service** , choisissez la catégorie de support appropriée. Vous devrez peut-être sélectionner **plus...** pour afficher des articles supplémentaires.

2. Complétez le formulaire de demande de service, puis sélectionnez **Envoyer**.

   > [!TIP]
   > Veillez à inclure vos coordonnées, et pas celles de votre client.

3. Ensuite, passez en revue les demandes de service de votre client en accédant au centre d’administration Office 365 et en sélectionnant **Afficher tous les tickets de support**.

### <a name="support-for-commercial-marketplace-products"></a>Prise en charge des produits de la place de marché commerciale

Microsoft ne fournit pas de support produit pour les produits de la place de marché commercial. Vous devez contacter l’éditeur de logiciels indépendant (ISV) qui a publié le produit pour bénéficier du support technique.

Pour trouver les coordonnées de l’ISV :

1.  Sur la page **Place de marché**, sélectionnez le produit pour lequel vous avez besoin d’aide.

2.  Sur la page du produit, vous trouverez des informations de contact du support technique. Il peut s’agir d’une ou plusieurs des options suivantes :

    - Lien vers un point d’entrée de support sur le site web de l’ISV
    - Adresse e-mail de support
    - Numéro de téléphone pour contacter le support

## <a name="faq"></a>Questions fréquentes (FAQ)

Consultez les questions fréquemment posées suivantes sur les demandes de service que vous pouvez envoyer pour le compte d’un client. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Qu’est-ce qui est inclus dans le droit au support&nbsp;?

Les demandes de service doivent être classées via l’espace partenaires. Ils sont disponibles pour Azure, Microsoft Office 365, Microsoft Dynamics CRM Online et Enterprise Mobility suite. En tant que partenaire participant au programme Fournisseur de solutions cloud, vous pouvez vous attendre à un temps de réponse prioritaire à vos problèmes majeurs.

La prise en charge de votre propre locataire partenaire n’est pas incluse dans le cadre de l’avantage du support CSP. Toutefois, Office 365, Microsoft Dynamics CRM Online et Enterprise Mobility suite ne sont pas facturés pour les partenaires ou les clients. Azure est facturé en payant, mais si vous êtes autorisé à la signature d’un support Cloud ou d’autres avantages d’Microsoft Partner Network (MPN), vous pouvez les utiliser pour payer ces frais.

Cet avantage s’applique à tous les partenaires qui participent au programme Fournisseur de solutions cloud, qu’ils aient un abonnement payant ou qu’ils soient en période d’essai. Le support pour la gestion des abonnements et de la facturation est également compris gratuitement dans ce package.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Quel est le délai pour obtenir une réponse initiale&nbsp;?

Le délai pour obtenir une première réponse dépend de la gravité du problème envoyé. La gravité d’un problème est déterminée par votre évaluation de l’impact sur votre activité lorsque vous envoyez une demande de service.

Temps de réponse initial pour les **incidents de réparation/réparation**:

- Impact critique (gravité A) : deux heures (perte ou dégradation significative des services). Interruption des services de production.)
- Impact modéré (gravité B) : quatre heures (perte modérée ou dégradation des services. Services de production partiellement affectés.)
- Impact minimal (gravité C) : huit heures (perte minimale ou dégradation des services). Les services sont toujours disponibles ou les services hors production sont affectés.)

Les délais de réponse initiale concernent uniquement le support en anglais. Le support en langue locale est fourni pendant les heures ouvrées.
Pour les incidents qui se situent dans les limites du droit de support, mais qui ne sont pas considérés comme des incidents de réparation, le temps de réponse initial peut être d’une journée de travail.

### <a name="can-i-submit-a-service-request-by-phone"></a>Puis-je envoyer une demande de service par téléphone&nbsp;?

Non, le support téléphonique n’est pas proposé pour ce programme.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Que se passe-t-il si je me connecte au portail Azure sans passer par l’Espace partenaires&nbsp;?

Si vous vous connectez directement au Portail Microsoft Azure, vous affichez le centre dans votre contexte, et non dans le contexte d’un client. C’est la raison pour laquelle vous devez vous connecter directement au Portail Microsoft Azure lors de la création d’une demande de service pour vos propres abonnements.

Le support technique de votre programme CSP ne prend pas en charge votre propre abonnement partenaire. Pour cette raison, vous devez fournir le droit de votre plan de support valide lorsque vous créez une demande de service qui concerne votre propre abonnement partenaire. Exemples : ID de contrat MPN, premier ou plan de support Azure. Pour plus d’informations, consultez le [Forum aux questions sur le support Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Que se passe-t-il si je me connecte au portail du centre d’administration Office 365 et que je ignore l’espace partenaires ?

Si vous vous connectez directement au centre d’administration Office 365, vous affichez le centre dans votre contexte, et non dans le contexte d’un client. C’est la raison pour laquelle vous devez vous connecter directement au centre d’administration Office 365 lors de la création d’une demande de service pour vos propres abonnements.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Comment obtenir un support Dynamics 365 supplémentaire ?

Si vous rencontrez des problèmes liés à : Dynamics 365 Planifiez les abonnements, les licences, la facturation, les opérations finance &, les licences Dynamics 365, ou vous avez besoin d’un support technique supplémentaire :
 
Contactez le [Support Dynamics](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Étapes suivantes

- [Fournir un support à vos clients](customer-support.md)
- [Vérifier l’état du service](check-service-health.md)
