---
title: Résoudre les problèmes liés à la configuration de votre compte espace partenaires ou à des problèmes de renouvellement MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Résolvez les problèmes lors de la tentative d’inscription dans l’espace partenaires. Répond aux défis avec les modes de paiement, les oublis de mots de passe et bien plus encore.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854687"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="0cf2d-104">Résoudre les problèmes de configuration de compte ou de renouvellement MPN</span><span class="sxs-lookup"><span data-stu-id="0cf2d-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="0cf2d-105">**Rôles appropriés**: administrateur général | Administrateur du partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="0cf2d-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="0cf2d-106">Voici quelques suggestions pour résoudre les problèmes courants qui surviennent lors de la configuration de votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="0cf2d-107">Que se passe-t-il si vous effectuez une migration à partir du centre d’appartenance au partenaire et que vous ne pouvez pas modifier les champs d’informations</span><span class="sxs-lookup"><span data-stu-id="0cf2d-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="0cf2d-108">Dans les cas où votre société a déjà une présence dans l’espace partenaires (par exemple, un compte CSP), un écran en lecture seule s’affiche.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="0cf2d-109">Cet écran affiche toutes les informations sur votre société telles qu’elles existent dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="0cf2d-110">Vous ne pouvez pas modifier les détails de cet écran.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-110">You can't change the details on this screen.</span></span> <span data-ttu-id="0cf2d-111">Cela est dû à la conception et non à une erreur.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-111">This is by design and not an error.</span></span>

<span data-ttu-id="0cf2d-112">Sélectionnez **accepter** et **Continuer** pour continuer.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="0cf2d-113">Si le service informatique a désactivé l' **inscription à l’espace partenaires**</span><span class="sxs-lookup"><span data-stu-id="0cf2d-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="0cf2d-114">Ce message s’affiche parce que les utilisateurs viraux sont désactivés ou parce que l’inscription virale est désactivée sur le locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="0cf2d-115">L’administrateur général de votre compte Azure AD peut activer les fonctionnalités requises en exécutant la commande PowerShell suivante :</span><span class="sxs-lookup"><span data-stu-id="0cf2d-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="0cf2d-116">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="0cf2d-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="0cf2d-117">Pour plus d’informations, consultez [inscription en libre-service](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="0cf2d-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="0cf2d-118">Vous avez oublié votre mot de passe</span><span class="sxs-lookup"><span data-stu-id="0cf2d-118">You forgot your password</span></span>

<span data-ttu-id="0cf2d-119">Si vous avez oublié votre mot de passe, sélectionnez le lien vous **ne pouvez pas accéder à votre compte ?** dans la page de connexion.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="0cf2d-120">Cette option vous permet de réinitialiser votre mot de passe ou de demander à votre administrateur général de vous attribuer de nouvelles informations d’identification.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="0cf2d-121">Sur l’écran « faites-nous part de votre entreprise », vous recevez une erreur « un problème est survenu »</span><span class="sxs-lookup"><span data-stu-id="0cf2d-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="0cf2d-122">Ce message d’erreur s’affiche généralement si vous utilisez par inadvertance des caractères spéciaux, des espaces ou un code de pays dans le numéro de téléphone de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="0cf2d-123">La valeur entrée dans le champ numéro de téléphone ne peut contenir que 10 caractères au maximum.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="0cf2d-124">Votre achat par carte de crédit reçoit un message d’erreur indiquant que la commande a été refusée.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="0cf2d-125">Veuillez vérifier vos informations»</span><span class="sxs-lookup"><span data-stu-id="0cf2d-125">Please verify your information”</span></span>


<span data-ttu-id="0cf2d-126">Utilisez toujours l’adresse correspondant à votre carte de crédit plutôt qu’à votre entité légale.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="0cf2d-127">En outre, assurez-vous que le code postal est correct et qu’il correspond à l’adresse que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="0cf2d-128">Vous souhaitez passer du paiement hors connexion au mode de paiement en ligne</span><span class="sxs-lookup"><span data-stu-id="0cf2d-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="0cf2d-129">Vous devez annuler la commande d’origine et effectuer un achat à l’aide du mode de paiement par défaut.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="0cf2d-130">Pour annuler une commande :</span><span class="sxs-lookup"><span data-stu-id="0cf2d-130">To cancel an order:</span></span>

1. <span data-ttu-id="0cf2d-131">Sélectionnez l’onglet **offres d’appartenance** dans le tableau de bord.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="0cf2d-132">Sélectionner **annuler la commande**</span><span class="sxs-lookup"><span data-stu-id="0cf2d-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="0cf2d-133">Une fenêtre de confirmation s’affiche et vous devez confirmer pour annuler la commande initiale.</span><span class="sxs-lookup"><span data-stu-id="0cf2d-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0cf2d-134">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0cf2d-134">Next steps</span></span>

- [<span data-ttu-id="0cf2d-135">Gérer votre compte dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0cf2d-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="0cf2d-136">Comment lire votre facture et votre fichier de rapprochement</span><span class="sxs-lookup"><span data-stu-id="0cf2d-136">How to read your bill and recon file</span></span>](read-your-bill.md)
