---
title: Impact des stratégies de taxes sur le paiement pour la place de marché Azure
description: Découvrez comment les stratégies de taxes affectent le paiement pour la place de marché Azure.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856013"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Impact des stratégies de taxes sur le paiement pour la place de marché Azure

**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent d’administration

## <a name="introduction"></a>Introduction

La place de marché commercial Microsoft a une portée mondiale. Les transactions se produisent dans les limites et selon l’emplacement de l’ISV et du client, les implications fiscales peuvent varier. Microsoft AppSource et la place de marché Azure utilisent les informations de profil fiscal de l’espace partenaires pour déterminer le pays de l’ISV. Pour déterminer le pays du client, utilisez les informations de facturation du client ou, si le client se trouve dans l’Union européenne, nous utilisons deux informations différentes.

Pour mieux comprendre les scénarios suivants, reportez-vous à la table des [Détails fiscaux](tax-details-marketplace.md) , qui indique si Microsoft collecte et paye les taxes pour le compte du serveur de publication ou si cette responsabilité appartient au serveur de publication.

> [!NOTE]
> Tous les exemples de valeurs de vente et de taxes dans cette rubrique sont fournis à titre d’illustration uniquement, pas des chiffres exacts.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Le serveur de publication transagit dans le pays d’imposition géré par Microsoft

**Scénario A** : transactions qui ont lieu entre un serveur de publication et un client dans un [pays d’imposition géré par Microsoft](tax-details-marketplace.md#microsoft-managed-countries). La taxe applicable sera ajoutée à ces transactions au moment de la vente et Microsoft envoie cette taxe au pays concerné. Aucun impôt n’est retenu du paiement et les calculs de paiement sont des taxes exclusives.

Consultez le [scénario D](#foreign-publisher-transacts-with-us-customer) pour les transactions entre un serveur de publication non US et un client américain.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Affiche le flux de travail pour le scénario de processus de paiement A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Le serveur de publication transagit dans un pays d’imposition géré par Microsoft, où les frais relatifs au marché sont imposables

**Scénario B** : transactions qui ont lieu entre un serveur de publication basé aux États-Unis (tel que défini par les informations de profil d’imposition de l’espace partenaires) à un client d’un pays d’imposition géré par Microsoft, où le pays impose une taxe sur les frais de la place de marché (un service imposable). Dans ce scénario, les taxes sur les frais de service du magasin sont soustraites du paiement de l’éditeur.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Affiche le flux de travail pour le scénario de processus de paiement B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Le serveur de publication transagit dans le pays d’imposition géré par l’éditeur

**Scénario C** : transactions qui ont lieu entre un serveur de publication et un client d’un pays d’imposition géré par un éditeur qui n’impose pas d’impôt à la retenue sur les clients. Les clients ne paient aucune taxe au point de vente et il s’agit de l’obligation de l’éditeur de payer toutes les taxes applicables.

Pour plus d’informations sur la tarification spécifique aux pays (par exemple, pour compenser la fiscalité à venir), consultez les [plans et la tarification des offres de la place de marché commercial](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Affiche le flux de travail pour le scénario de processus de paiement C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Le serveur de publication étranger transagit avec le client US

**Scénario D** : tous les serveurs de publication étrangers (tels que définis par leurs informations de profil d’imposition de l’espace partenaires) dans les pays sans traité des États-Unis (voir le [scénario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) faisant une vente à un client basé aux États-Unis (comme défini par l’adresse de son compte client). Le gouvernement des États-Unis requiert que Microsoft retenu la taxe de la part du serveur de publication. Les taxes retenues du paiement au serveur de publication sont calculées en fonction du prix de l’offre.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Affiche le flux de travail du scénario de processus de paiement D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Un serveur de publication étranger avec un traité transagit avec le client américain

**Scénario E** : tous les serveurs de publication étrangers (tels que définis par leurs informations de profil d’imposition de l’espace partenaires) dans les pays avec un traité des États-Unis faisant l’acquisition d’une vente à un client basé aux États-Unis (comme défini par l’adresse de son compte client). Le gouvernement des États-Unis ne demande pas à Microsoft de retenir une taxe pour le compte du serveur de publication.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Affiche le flux de travail du scénario de processus de paiement E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Le serveur de publication étranger vend à un client inscrit à la TVA UE dans un pays géré par Microsoft (en dehors de l’Irlande)

**Scénario F** : toutes les transactions entre les éditeurs étrangers et les clients inscrits à la TVA UE (en dehors de l’Irlande) dans un pays Microsoft-Managed. Le client ne paie pas d’impôt sur la vente.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Affiche le flux de travail du scénario de processus de paiement F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Le serveur de publication étranger vend à un client inscrit à la TVA UE dans un pays géré par Microsoft (en Irlande)

**Scénario G** – toutes les transactions entre les serveurs de publication étrangers et les clients inscrits à la TVA UE (à l’Irlande) dans un Microsoft-Managed pays. Le client paie la TVA irlandaise et Microsoft paie cette taxe au gouvernement irlandais.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Affiche le flux de travail du scénario de processus de paiement G.":::

## <a name="next-steps"></a>Étapes suivantes

- [FAQ sur l’éditeur](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instructions pour créer des profils de paiement et de taxes](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)