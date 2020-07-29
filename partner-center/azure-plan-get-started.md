---
title: Commencer votre transfert vers le plan Azure
description: Découvrez ce que vous et vos clients devez savoir sur l’utilisation du plan de paiement à l’utilisation Azure, notamment les premières étapes, les précautions de sécurité et comment démarrer.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: cf2d1085b529e1fbd0fad74c4e56d16f789a48e9
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943956"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Commencer à pratiquer les prix de paiement à l’utilisation avec le plan Azure

Microsoft a introduit une nouvelle expérience de commerce dans l’Espace partenaires.  Cette nouvelle expérience de commerce donne aux partenaires l’accès aux services Azure à un tarif de paiement à l’utilisation pour les clients dans le cadre du Contrat client Microsoft.

Ce plan simplifie l’expérience d’achat et vous pouvez avoir plusieurs abonnements Azure dans un plan Azure. Vous n’avez plus besoin d’envoyer une commande distincte par abonnement Azure. De plus, dans cette nouvelle expérience de commerce pour Azure, nous nous sommes alignés sur un principe unique de tarification globale permettant aux partenaires fournisseurs de solutions Cloud de proposer Azure aux prix publiés.

Les besoins liés à la transformation numérique de nos clients requièrent de nouvelles compétences des partenaires. De nombreux clients recherchent des partenaires capables de fournir des services dépassant une simple transaction, qui pourront assouplir leur adoption du cloud et les aider à consommer efficacement les services Azure. Les partenaires Microsoft jouent un rôle essentiel dans toutes les phases du cycle de vie du client. Les services de partenaire de ce type sont continus par nature et incluent la surveillance du patrimoine, la gestion des stratégies et de la gouvernance, le réglage précis de l’installation et de la configuration, le support technique et un large éventail d’autres services. Le partenaire doit très bien connaître l’environnement Azure du client. De plus, il doit disposer d’une gouvernance et d’un contrôle continus et appropriés des ressources sous-jacentes qu’il gère. Un partenaire de facturation qui assure cette gestion des opérations cloud 24 h/24 et 7 j/7 devient éligible pour bénéficier d’un **crédit Partenaires pour services managés** pour cette activité.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>S’assurer que les clients ont signé le Contrat client Microsoft

Depuis le 1er octobre 2019, le Contrat client Microsoft, un contrat perpétuel qui simplifie et rationalise l’expérience d’achat des clients avec un processus entièrement numérique, est disponible. Tous les clients qui souhaitent tirer parti de la nouvelle expérience de commerce dans le cadre du programme Fournisseur de solutions Cloud pour Azure doivent signer le Contrat client Microsoft.

Les partenaires souhaitant effectuer leurs transactions sous le nouveau plan Azure et passer une nouvelle commande doivent confirmer que les clients acceptent le Contrat client Microsoft en utilisant l’API en production et le tableau de bord de l’Espace partenaires.

À partir du 1er février 2020, le contrat Microsoft Cloud existant sera supprimé du programme CSP. À compter de ce jour, la confirmation (attestation) du partenaire que les clients acceptent le nouveau contrat client Microsoft sera obligatoire pour toutes les autres offres, notamment Microsoft 365, Dynamics 365 et les offres Azure existantes. Les partenaires du programme CSP ne pourront pas passer de nouvelle commande pour les clients sans attestation du Contrat client Microsoft.

Pour plus d’informations, lisez [Confirmer l’acceptation du Contrat client Microsoft par le client](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Pratiques de sécurité et de contrôle d’accès

Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires participant au programme Fournisseur de solutions Cloud.

Les partenaires qui n’implémentent pas les exigences de sécurité obligatoires ne seront pas en mesure d’effectuer des transactions dans le cadre du programme Fournisseur de solutions Cloud ou de gérer les locataires clients en tirant parti des droits d’administrateur délégué, une fois ces exigences appliquées. Nous sommes en train de mettre en place une date de mise en œuvre technique pour les exigences et notifieront les partenaires de la date avec des informations détaillées.

## <a name="actions-to-take-to-implement-mfa"></a>Actions à entreprendre pour implémenter l’authentification multifacteur

Étant donné la nature hautement privilégiée de la qualité de partenaire, nous devons nous assurer que chaque utilisateur a un test MFA pour chaque authentification unique. Pour ce faire, vous pouvez procéder de l’une des façons suivantes :

- Implémentation d’Azure AD Premium et vérification de l’application de l’authentification multifacteur (MFA) pour chaque utilisateur
- Implémentation des [paramètres de sécurité par défaut d’Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implémentation d’une solution tierce et vérification de l’application de l’authentification multifacteur pour chaque utilisateur

Depuis le 1er août 2019, tous les partenaires doivent mettre en œuvre l’authentification multifacteur pour tous les utilisateurs, y compris les comptes de service, dans leur locataire de partenaire. Vous trouverez des informations détaillées sur ces exigences de sécurité dans [Exigences de sécurité des partenaires](partner-security-requirements.md).

Microsoft recommande aux partenaires d’utiliser RBAC en toute diligence, en suivant les bonnes pratiques mises en œuvre via les [ressources Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>En savoir plus sur le plan Azure

- [Acheter le plan Azure](purchase-azure-plan.md)

- [Comparer les offres Azure](compare-azure-offers.md)

- [Crédit Partenaires – Vue d’ensemble](partner-earned-credit.md)

- Les calculs de crédit Partenaires, et les rôles et autorisations qui sont éligibles pour obtenir des crédits Partenaires, sont disponibles dans la liste des tarifs du tableau de bord de l’Espace partenaires (connexion requise).

## <a name="next-steps"></a>Étapes suivantes 

- [Détermination du crédit Partenaires – Détails](partner-earned-credit-explanation.md)
- [Explication des tarifs du plan Azure](azure-plan-price-list.md)
- [Gérer la transition de vos clients vers le plan Azure](azure-plan-transition.md)
- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)
- [Liste complète des pays/régions où le plan Azure est disponible](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)
