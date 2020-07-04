---
title: S’inscrire au programme Fournisseur de solutions Cloud
ms.topic: article
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.date: 06/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En savoir plus sur les exigences du programme CSP pour les partenaires qui souhaitent s’inscrire au programme fournisseur de solutions Cloud pour Microsoft Cloud pour le gouvernement des États-Unis.
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 67dd4823e5167fb0e0ece692e873cd8cde7013ea
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947540"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Inscrivez-vous au programme fournisseur de solutions Cloud pour Microsoft Cloud pour le gouvernement des États-Unis

**S’applique à**

- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Administrateur général

Les partenaires Microsoft peuvent désormais vendre des solutions et services Cloud Microsoft aux entités américaines Federal, State, local et tribales par le biais du programme fournisseur de solutions Cloud (CSP) pour les Microsoft Cloud pour le gouvernement des États-Unis. 

Microsoft Cloud pour le gouvernement des États-Unis fournit une instance privée, dédiée et isolée de Microsoft Azure qui répond aux exigences du gouvernement des États-Unis en matière de sécurité, de confidentialité et de conformité des données. Votre entreprise doit respecter les conditions d’éligibilité de Microsoft pour participer au programme CSP pour Microsoft Cloud pour le gouvernement des États-Unis. Pour plus d’informations, consultez [Partner Center for Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md).

## <a name="before-you-begin"></a>Avant de commencer

Avant de pouvoir vous inscrire au programme CSP pour Microsoft Cloud pour le gouvernement des États-Unis, nous devons vérifier que votre entreprise répond aux conditions de vente aux entités gouvernementales américaines. Avant de lancer le processus d’inscription, remplissez le formulaire de [validation Cloud Microsoft Government](https://azuregov.microsoft.com/csp) afin de pouvoir vérifier l’éligibilité de votre entreprise. Une fois que nous avons vérifié l’éligibilité de votre entreprise, nous vous fournissons un locataire Azure Active Directory (Azure AD) propre au Microsoft Cloud pour le gouvernement des États-Unis.  

Pour créer un compte espace partenaires et s’inscrire auprès du fournisseur CSP pour Microsoft Cloud pour le gouvernement des États-Unis, vous devez fournir les informations suivantes (vous pouvez rassembler ces informations avant de lancer le processus d’inscription) :

-  Informations d’identification d’administrateur général pour le nouveau locataire Azure AD de votre organisation pour Microsoft Cloud pour le gouvernement des États-Unis
-  ID d’Microsoft Partner Network (MPN) de votre organisation 
-  Une adresse professionnelle dans le États-Unis

> [!IMPORTANT]  
> Si vous avez un compte existant dans l’espace partenaires et que vous souhaitez vous inscrire au CSP pour Microsoft Cloud pour le gouvernement des États-Unis, vous devez créer un nouveau compte distinct pour le marché du gouvernement des États-Unis.

## <a name="how-to-enroll"></a>Procédure d'inscription 

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Étape 1 : créer un compte espace partenaires pour Microsoft Cloud pour le gouvernement des États-Unis

1.  Lancez le processus d’inscription [ici](https://partnercenter.microsoft.com/register/resellerusgjoinnow). 

2.  Connectez-vous avec les informations d’identification d’administrateur général pour le locataire Azure AD de votre organisation pour Microsoft Cloud pour le gouvernement des États-Unis. Si votre organisation n’a pas de compte pour ce portail, vous pouvez en demander une en suivant le [formulaire de validation Cloud Microsoft Government](https://azuregov.microsoft.com/csp).


### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Étape 2 : demander à participer au programme fournisseur de solutions Cloud pour Microsoft Cloud pour le gouvernement des États-Unis

1.  Renseignez les informations manquantes sur le formulaire d’inscription, y compris votre ID de Microsoft Partner Network et les détails du support technique de votre organisation. 

2.  Sélectionnez **Accepter et continuer**. L'examen de votre demande peut nous prendre plusieurs jours. Nous vous enverrons un e-mail lorsque nous en aurons terminé.

    > [!IMPORTANT]  
    > En sélectionnant **accepter et continuer**, vous confirmez que vous êtes autorisé à agir au nom de votre organisation et que vous acceptez d’autoriser Microsoft à exécuter une vérification de solvabilité en arrière-plan avant de passer en revue l’application de fournisseur de solutions Cloud de votre organisation.


### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Étape 3 : signer le contrat du revendeur pour Microsoft Cloud pour le gouvernement des États-Unis

1. Connectez-vous à l’espace partenaires pour Microsoft Cloud pour le gouvernement des États-Unis à l’aide du lien fourni dans le message d’approbation de l’application. 

2. Sur la page **contrat** , lisez les termes et, si vous en acceptez, sélectionnez **accepter et continuer** pour signer numériquement le [contrat de revendeur pour Microsoft Cloud pour le gouvernement des États-Unis](https://go.microsoft.com/fwlink/p/?linkid=843364). La création de votre compte peut prendre plusieurs heures. Déconnectez-vous du Centre des partenaires pour Microsoft Cloud pour le gouvernement des États-Unis, puis reconnectez-vous ultérieurement.


### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Étape 4 : affecter des utilisateurs au rôle de l’agent admin dans le portail d’administration Microsoft Azure pour Microsoft Cloud pour le gouvernement des États-Unis

Microsoft Cloud pour le gouvernement des États-Unis fournit une instance distincte de Microsoft Azure qui respecte les normes de conformité, de sécurité et de confidentialité du gouvernement. Pour permettre aux administrateurs de gérer les utilisateurs et les licences dans le Portail Microsoft Azure, vous devez leur attribuer manuellement le rôle d’agent d’administration.

> [!NOTE]  
> Une fois que vous avez affecté des utilisateurs au rôle d’agent administrateur, ils peuvent accéder à la liste de vos clients sur la page **clients** et [ajouter de nouveaux clients](add-a-new-customer.md).   

1.  Connectez-vous au portail d’administration Microsoft Azure à l’adresse https://portal.azure.us/ .

2.  Affectez le rôle d’agent d’administration aux utilisateurs appropriés de votre organisation. Pour ce faire, vous devez ajouter ces utilisateurs au groupe **AdminAgent** intégré. Pour plus d’informations sur la procédure à suivre, consultez [gérer les membres d’un groupe dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-groups-members-azure-portal) .
 
## <a name="connect-with-us"></a>Rejoignez-nous

- Des questions ? Envoyez-nous un e-mail à l’adresseazgovcsp@microsoft.com

- Rejoignez-nous sur [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777&view=all) 

## <a name="related-topics"></a>Rubriques connexes

-  [Espace partenaires de Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md)

-  [Gestion des utilisateurs et des licences dans l’Espace partenaires pour Microsoft Cloud for US Government](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)


