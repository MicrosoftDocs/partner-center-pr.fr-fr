---
title: Clients Azure ActiveDirectory et Espace partenaires | Espace partenaires
description: "Pour créer un compte Espace partenaires, votre entreprise doit avoir un client Azure ActiveDirectory (AzureAD). AzureAD est le service d’annuaire et de gestion des identités basé sur le cloud de Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Clients Azure ActiveDirectory et Espace partenaires  

**S’applique à**

-  Espace partenaires

## <a name="why-you-need-an-azure-ad-tenant"></a>Pourquoi un client AzureAD est-il nécessaire?

Nous devons associer le client AzureAD de votre entreprise à votre nouveau compte Espace partenaires, afin que vos utilisateurs clients soient en mesure de se connecter à l’Espace partenaires à l’aide de leur nom d’utilisateur et mot de passe AzureAD (compte Microsoft).

Si votre entreprise dispose déjà d’un client AzureAD, vous pouvez l’associer à votre compte Espace partenaires. 

>**Remarque**<br> Avant de décider d’utiliser un client AzureAD existant, tenez compte du nombre d’utilisateurs du client devant travailler dans l’Espace partenaires. Si certains utilisateurs du client n’ont pas besoin de travailler dans l’Espace partenaires, envisagez de créer un nouveau client dédié aux utilisateurs appelés à travailler dans l’Espace partenaires.

Si votre entreprise n’a pas encore de client AzureAD, vous pouvez en créer un gratuitement lors de l’inscription. Sélectionnez **Créer un nouveau client** sur la page **Se connecter à Azure ActiveDirectory**. 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Vous ne savez pas si votre entreprise a déjà un client AzureAD?

Si vous ignorez si votre entreprise dispose d’un client AzureAD, procédez comme suit pour le vérifier. Notez que si vous avez un abonnement actif à MicrosoftAzure ou Office365, vous disposez déjà d’un client AzureAD.
1.  Ouvrez une session depuis le portail d’administration Azure à l’adresse https://ms.portal.azure.com
2.  Dans le menu, sélectionnez Azure ActiveDirectory, puis Noms de domaine.
3.  Si vous disposez déjà d’un client, votre nom de domaine est répertorié dans la liste.

### <a name="using-an-existing-tenant"></a>Vous voulez utiliser un client existant?

Si vous souhaitez utiliser un client AzureAD existant, mais que vous rencontrez des problèmes de connexion, recherchez le scénario correspondant le mieux à votre situation dans le diagramme ci-dessous et suivez les étapes recommandées. 

![Vous disposez d’un client AzureAD ou vous devez en créer un?](images/onboardingAADFlow.png)

Pour plus d’informations sur l’ajout de domaines dans AzureAD, voir [Ajouter ou associer un domaine dans AzureAD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>À propos de MicrosoftAzure

MicrosoftAzure est une plateforme cloud publique que les entreprises peuvent utiliser pour créer, déployer et gérer des applications sur un réseau global de centres de données gérés par Microsoft. Les entreprises utilisent Azure pour créer une infrastructure informatique virtuelle dotée de fonctions ou de services virtuels, au lieu d’ordinateurs physiques. 

Lorsque vous achetez un abonnement Azure, vous louez de fait un espace sécurisé dédié dans le cloud public Azure, comme vous pouvez louer des locaux dans un immeuble de bureaux pour y héberger physiquement votre entreprise. Votre entreprise est client du propriétaire de l’immeuble de bureaux. 

Un client AzureAD est une représentation virtuelle dédiée et isolée de votre entreprise dans le cloud public Azure. Il est créé pour vous lorsque vous vous abonnez à un service de cloud computing Microsoft tel qu’Azure, MicrosoftIntune ou Office365. 

Votre client héberge vos utilisateurs AzureAD et les informations les concernant telles que leur mot de passe, les données de profil, les autorisations et autres informations. Le client contient également les groupes, les applications et toutes les informations relatives à une entreprise et à sa sécurité. 

Pour en savoir plus sur AzureAD, consultez la [documentation Azure ActiveDirectory](https://docs.microsoft.com/ azure/active-directory/). 