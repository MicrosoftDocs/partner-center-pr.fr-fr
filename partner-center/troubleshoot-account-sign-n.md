---
title: Résoudre les problèmes liés à la configuration de votre compte espace partenaires ou à des problèmes de renouvellement MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Résoudre les problèmes liés à l’inscription dans l’espace partenaires
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848933"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="50434-103">Résoudre les problèmes de configuration de compte ou de renouvellement MPN</span><span class="sxs-lookup"><span data-stu-id="50434-103">Troubleshoot account setup or MPN renewal issues</span></span>

### <a name="applies-to"></a><span data-ttu-id="50434-104">S’applique à</span><span class="sxs-lookup"><span data-stu-id="50434-104">Applies to</span></span>

- <span data-ttu-id="50434-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="50434-105">Partner Center</span></span>
 
### <a name="appropriate-roles"></a><span data-ttu-id="50434-106">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="50434-106">Appropriate roles</span></span>

- <span data-ttu-id="50434-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="50434-107">Global admin</span></span>
- <span data-ttu-id="50434-108">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="50434-108">MPN partner admin</span></span> 
 

<span data-ttu-id="50434-109">Voici quelques suggestions pour résoudre les problèmes courants qui surviennent lors de la configuration de votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="50434-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="50434-110">Que se passe-t-il si vous effectuez une migration à partir du centre d’appartenance au partenaire et que vous ne pouvez pas modifier les champs d’informations</span><span class="sxs-lookup"><span data-stu-id="50434-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="50434-111">Cela se produit dans les cas où votre société a déjà une présence dans l’espace partenaires (par exemple, le compte CSP). vous verrez alors un écran en lecture seule qui affiche toutes les informations relatives à votre société telles qu’elles existent dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="50434-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="50434-112">Vous ne pouvez pas modifier les détails de cet écran.</span><span class="sxs-lookup"><span data-stu-id="50434-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="50434-113">Cela est dû à la conception et non à une erreur.</span><span class="sxs-lookup"><span data-stu-id="50434-113">This is by design and not an error.</span></span>

<span data-ttu-id="50434-114">Sélectionnez **accepter** et **Continuer** pour continuer.</span><span class="sxs-lookup"><span data-stu-id="50434-114">Select **Accept** and **Continue** to proceed.</span></span>

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="50434-115">Vous essayez d’inscrire ou de migrer à partir du centre d’appartenance au partenaire. vous recevez un message d’erreur indiquant que le service informatique a désactivé l' **inscription à l’espace partenaires**.</span><span class="sxs-lookup"><span data-stu-id="50434-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span> 

<span data-ttu-id="50434-116">Ce message s’affiche parce que les utilisateurs viraux sont désactivés ou que l’inscription virale est désactivée sur le locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50434-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="50434-117">L’administrateur général de votre compte Azure AD peut activer les fonctionnalités requises en exécutant la commande PowerShell suivante :</span><span class="sxs-lookup"><span data-stu-id="50434-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="50434-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="50434-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="50434-119">Pour plus d’informations, consultez [inscription en libre-service](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="50434-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

### <a name="you-forgot-your-password"></a><span data-ttu-id="50434-120">Vous avez oublié votre mot de passe</span><span class="sxs-lookup"><span data-stu-id="50434-120">You forgot your password</span></span>

<span data-ttu-id="50434-121">Si vous avez oublié votre mot de passe, sélectionnez le lien vous **ne pouvez pas accéder à votre compte ?** sur la page de connexion pour réinitialiser votre mot de passe ou demandez à votre administrateur général de vous attribuer de nouvelles informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="50434-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="50434-122">Sur l’écran « faites-nous part de votre société », vous recevez une erreur « un problème est survenu »</span><span class="sxs-lookup"><span data-stu-id="50434-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="50434-123">Cela se produit généralement si vous utilisez par inadvertance des caractères spéciaux, des espaces ou du code de pays dans le numéro de téléphone de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="50434-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="50434-124">La valeur entrée dans le champ numéro de téléphone ne peut contenir que 10 caractères au maximum.</span><span class="sxs-lookup"><span data-stu-id="50434-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="50434-125">Vous essayez de terminer l’achat par carte de crédit, mais vous recevez un message d’erreur indiquant que la commande a été refusée.</span><span class="sxs-lookup"><span data-stu-id="50434-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="50434-126">Veuillez vérifier vos informations»</span><span class="sxs-lookup"><span data-stu-id="50434-126">Please verify your information”</span></span>

<span data-ttu-id="50434-127">Vous devez toujours insérer l’adresse correspondant à votre carte de crédit et ne correspond pas à votre entité légale.</span><span class="sxs-lookup"><span data-stu-id="50434-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="50434-128">En outre, assurez-vous que le code postal est correct et qu’il correspond à l’adresse que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="50434-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="50434-129">Vous souhaitez passer du paiement hors connexion au mode de paiement en ligne</span><span class="sxs-lookup"><span data-stu-id="50434-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="50434-130">Vous devez annuler la commande d’origine et effectuer un achat à l’aide du mode de paiement par défaut.</span><span class="sxs-lookup"><span data-stu-id="50434-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="50434-131">Pour annuler une commande :</span><span class="sxs-lookup"><span data-stu-id="50434-131">To cancel an order:</span></span>

1. <span data-ttu-id="50434-132">Sélectionnez l’onglet **offres d’appartenance** dans le tableau de bord.</span><span class="sxs-lookup"><span data-stu-id="50434-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="50434-133">Sélectionner **annuler la commande**</span><span class="sxs-lookup"><span data-stu-id="50434-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="50434-134">Une fenêtre de confirmation s’affiche et vous devez confirmer pour annuler la commande initiale.</span><span class="sxs-lookup"><span data-stu-id="50434-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
