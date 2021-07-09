---
title: Demander un crédit de contrat SLA à Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Découvrez les avantages, les restrictions et les procédures pour demander un crédit de contrat de niveau de service (SLA) auprès de Microsoft si vos clients rencontrent une panne de service.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519441"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Comment et quand demander un crédit de contrat de niveau de service (SLA) de Microsoft

**Rôles appropriés**: agent admin | Administrateur général

Vous pouvez demander des **crédits de contrat de niveau de service (SLA)** auprès de Microsoft si un service que vous fournissez à vos clients présente une panne.

## <a name="sla-credit-calculation"></a>Calcul du crédit SLA

Les crédits SLA de Microsoft sont déterminés en fonction du ou des services qui ont été affectés. par exemple, si votre client dispose d’une Office 365 suite, mais qu’une panne de SharePoint s’est produite, le crédit du contrat SLA est approuvé uniquement pour les SharePoint et non pour l’ensemble du plan du client.

*Les crédits sont évalués au prorata en fonction du service affecté et de la durée de la panne.* Pour connaître les types de scénarios qui sont éligibles pour les crédits du contrat SLA, consultez le document sur les [services en ligne du contrat SLA consolidé](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). ces informations s’appliquent également aux services vendus par le biais du programme de fournisseur de solutions Cloud (CSP).


## <a name="request-an-sla-credit"></a>Demander un crédit SLA

*Le partenaire CSP doit soumettre la réclamation et toutes les informations requises à la fin du mois civil suivant le mois au cours duquel l’incident s’est produit.* Par exemple, si l’incident s’est produit le 15 février, Microsoft doit recevoir la revendication et toutes les informations requises avant le 31 mars. Les clients finaux et les revendeurs indirects ne peuvent pas soumettre des demandes de crédit du contrat SLA. le fournisseur indirect ou le partenaire direct Bill doit soumettre des revendications en son nom.

> [!NOTE]
> Les incidents de Conseil ne sont généralement pas éligibles pour les crédits SLA. Un incident publié dans le tableau de bord Service Health indique qu’un locataire peut être affecté et représente les meilleures informations *que* Microsoft a au moment de la publication. Les données de la page d’intégrité représentent la disponibilité générale d’un service. L’impact, l’atténuation et la résolution des services individuels peuvent varier. Pour plus d’informations, consultez le billet final de l’incident et la révision après incident. pour plus d’informations, consultez [comment vérifier Microsoft 365 service health](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) .

### <a name="required-information"></a>Informations requises

Le nom du client, l’identificateur du locataire, le ticket de partenaire # et l’horodatage de date/heure de création du ticket ne sont pas suffisants pour traiter une revendication.

Avant de [soumettre une demande de crédit SLA](#submit-sla-credit-request) à Microsoft, vous devez rassembler **toutes** les informations suivantes à inclure dans votre ticket de support :

- GUID du locataire client
- L' [identificateur](#outage-incident-identifier)de l’incident de panne ?
- Preuve que le client a été affecté par la panne et a demandé un crédit SLA.
- Les abonnements concernés ont-ils été achetés par le biais du CSP ? (*Oui* ou *non*)

#### <a name="evidence-that-proves-customer-impact"></a>Preuve qui prouve l’impact du client

- Informations relatives à l’heure et à la durée du temps d’arrêt
- Le nombre et le ou les emplacements des utilisateurs affectés (le cas échéant)
- Descriptions de vos tentatives de résolution de l’incident au moment de l’occurrence
- Un e-mail du client affecté demandant le support et par la suite
- Le numéro de ticket de support et les détails du contact client en ce qui concerne la résolution de l’impact du service


#### <a name="outage-incident-identifier"></a>Identificateur de l’incident de panne

vous pouvez trouver l’identificateur de l’incident de panne sur la page **Service Health** du Centre d’administration Microsoft 365. l' **ID d’Incident de panne** est un nombre précédé d’une abréviation à deux lettres qui indique le service affecté (par exemple, *EX25194* pour une panne Exchange Online). Le tableau suivant décrit les abréviations de service courantes :

| Abréviation à deux lettres | Service Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype Entreprise En ligne (anciennement Lync Online) |
| Système d''exploitation | Abonnement Office |
| Po | Power BI pour Office 365 |
| SP | SharePoint Online |
| Ye | Yammer Entreprise |
| MO | Erreur du portail |

### <a name="submit-sla-credit-request"></a>Envoyer une demande de crédit SLA

Pour envoyer votre demande de crédit SLA à Microsoft via le tableau de bord de l’espace partenaires :

1. Connectez-vous au tableau de bord de l’Espace partenaires.
2. Dans le menu de gauche, choisissez **demandes de service**, puis sélectionnez **demandes de support de partenaire**.
3. Sur la page **demande de partenaire** , choisissez **nouvelle requête**.
4. Dans la page **Démarrer la demande** , recherchez la section **CSP-Customers, Orders et subscriptions**. Dans cette section, choisissez **Sélectionner un type de problème**, puis sélectionnez **demandes de crédit de services client**.
5. Dans la page **solutions recommandées** , sous avez **-vous besoin d’aide supplémentaire ?**, choisissez **Oui**.
6. Dans la page **Détails** , renseignez la section **Détails du problème** . Dans la zone de texte **Détails** , veillez à entrer les [informations requises](#required-information) que vous avez rassemblées précédemment.
7. Choisissez **Envoyer** pour envoyer dans votre demande de crédit SLA.

## <a name="next-steps"></a>Étapes suivantes

- [Signaler des problèmes pour le compte de votre client](report-problems-on-behalf-of-a-customer.md)
