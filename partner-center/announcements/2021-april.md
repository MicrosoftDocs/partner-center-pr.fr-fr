---
title: Annonces d’avril 2021
description: Annonces du mois d’avril 2021 pour l’Espace partenaires Microsoft, avec notamment les nouvelles fonctionnalités, les promotions, les offres, les marchés ou les changements apportés aux offres existantes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702822"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="fcad0-103">Annonces d’avril 2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-103">April 2021 announcements</span></span>

<span data-ttu-id="fcad0-104">Cette page contient les annonces de l’Espace partenaires Microsoft d’avril 2021.</span><span class="sxs-lookup"><span data-stu-id="fcad0-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="fcad0-105">Préparation : Mise à jour de l’API de validation des adresses client CSP en juin - Fonctionnalité de test disponible dès maintenant</span><span class="sxs-lookup"><span data-stu-id="fcad0-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-106">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-106">Categories</span></span>

- <span data-ttu-id="fcad0-107">Date : 30/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="fcad0-108">Préparation</span><span class="sxs-lookup"><span data-stu-id="fcad0-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-109">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-109">Summary</span></span>

<span data-ttu-id="fcad0-110">Pour aider nos partenaires et nos clients à gérer leur entreprise en toute confiance, nous les invitons à tester les modifications qui ont été apportées à l’API de validation des adresses, disponible pour le monde entier.</span><span class="sxs-lookup"><span data-stu-id="fcad0-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-111">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-111">Impacted audience</span></span>

<span data-ttu-id="fcad0-112">Les partenaires à facturation directe CSP et les fournisseurs indirects qui créent ou mettent à jour l’adresse de clients existants</span><span class="sxs-lookup"><span data-stu-id="fcad0-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-113">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-113">Details</span></span>

<span data-ttu-id="fcad0-114">Chez Microsoft, la confiance est notre priorité.</span><span class="sxs-lookup"><span data-stu-id="fcad0-114">Microsoft runs on trust.</span></span> <span data-ttu-id="fcad0-115">Nous nous engageons à fournir une méthode de validation des adresses clients qui soit conforme, sûre et sécurisée pour les transactions liées aux abonnements des clients dans le cadre du programme Fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="fcad0-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="fcad0-116">Depuis le 31 mars 2021, nous avons apporté des modifications à l’API de validation des adresses.</span><span class="sxs-lookup"><span data-stu-id="fcad0-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="fcad0-117">Nous invitons les partenaires à tester l’API avant sa mise en ligne à la fin du mois de juin 2021.</span><span class="sxs-lookup"><span data-stu-id="fcad0-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="fcad0-118">Notez que ces modifications affectent uniquement l’API de validation des adresses.</span><span class="sxs-lookup"><span data-stu-id="fcad0-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="fcad0-119">Les API de création de client et de mise à jour du profil de facturation ne sont pas affectées.</span><span class="sxs-lookup"><span data-stu-id="fcad0-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="fcad0-120">Même s’il n’est pas obligatoire d’utiliser l’adresse suggérée avec l’API de création de client, il est vivement recommandé de le faire.</span><span class="sxs-lookup"><span data-stu-id="fcad0-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="fcad0-121">La réponse renverra l’un des messages d’état suivants :</span><span class="sxs-lookup"><span data-stu-id="fcad0-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="fcad0-122">Statut</span><span class="sxs-lookup"><span data-stu-id="fcad0-122">Status</span></span>     | <span data-ttu-id="fcad0-123">Description</span><span class="sxs-lookup"><span data-stu-id="fcad0-123">Description</span></span> |    <span data-ttu-id="fcad0-124">Nombre d’adresses suggérées retournées</span><span class="sxs-lookup"><span data-stu-id="fcad0-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="fcad0-125">Verified shippable (Valide pour l’expédition)</span><span class="sxs-lookup"><span data-stu-id="fcad0-125">Verified shippable</span></span> | <span data-ttu-id="fcad0-126">L’adresse est vérifiée, et valide en tant qu’adresse d’expédition.</span><span class="sxs-lookup"><span data-stu-id="fcad0-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="fcad0-127">Unique</span><span class="sxs-lookup"><span data-stu-id="fcad0-127">Single</span></span> |
|<span data-ttu-id="fcad0-128">Verified</span><span class="sxs-lookup"><span data-stu-id="fcad0-128">Verified</span></span> | <span data-ttu-id="fcad0-129">L’adresse est vérifiée.</span><span class="sxs-lookup"><span data-stu-id="fcad0-129">Address is verified.</span></span> | <span data-ttu-id="fcad0-130">Unique</span><span class="sxs-lookup"><span data-stu-id="fcad0-130">Single</span></span> |
|<span data-ttu-id="fcad0-131">Interaction required (Interaction nécessaire)</span><span class="sxs-lookup"><span data-stu-id="fcad0-131">Interaction required</span></span> | <span data-ttu-id="fcad0-132">L’adresse suggérée est très différente de la précédente et nécessite une confirmation de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="fcad0-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="fcad0-133">Unique</span><span class="sxs-lookup"><span data-stu-id="fcad0-133">Single</span></span> |
|<span data-ttu-id="fcad0-134">Street partial (Informations sur la voie incomplètes)</span><span class="sxs-lookup"><span data-stu-id="fcad0-134">Street partial</span></span> | <span data-ttu-id="fcad0-135">La rue donnée dans l’adresse est partielle et nécessite davantage d’informations.</span><span class="sxs-lookup"><span data-stu-id="fcad0-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="fcad0-136">Multiple (maximum trois)</span><span class="sxs-lookup"><span data-stu-id="fcad0-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="fcad0-137">Premises partial (Informations sur le bâtiment incomplètes)</span><span class="sxs-lookup"><span data-stu-id="fcad0-137">Premises partial</span></span> | <span data-ttu-id="fcad0-138">Les informations fournies sur le bâtiment (numéro de bâtiment, numéro de suite, etc.) sont incomplètes.</span><span class="sxs-lookup"><span data-stu-id="fcad0-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="fcad0-139">Multiple (maximum trois)</span><span class="sxs-lookup"><span data-stu-id="fcad0-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="fcad0-140">Multiple</span><span class="sxs-lookup"><span data-stu-id="fcad0-140">Multiple</span></span> | <span data-ttu-id="fcad0-141">Plusieurs champs sont incomplets dans l’adresse (notamment ceux concernant la voie et le bâtiment).</span><span class="sxs-lookup"><span data-stu-id="fcad0-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="fcad0-142">Multiple (maximum trois)</span><span class="sxs-lookup"><span data-stu-id="fcad0-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="fcad0-143">Aucun</span><span class="sxs-lookup"><span data-stu-id="fcad0-143">None</span></span> | <span data-ttu-id="fcad0-144">L’adresse est incorrecte.</span><span class="sxs-lookup"><span data-stu-id="fcad0-144">Address is incorrect.</span></span> | <span data-ttu-id="fcad0-145">Aucun</span><span class="sxs-lookup"><span data-stu-id="fcad0-145">None</span></span> |
|<span data-ttu-id="fcad0-146">Non validée</span><span class="sxs-lookup"><span data-stu-id="fcad0-146">Not validated</span></span> | <span data-ttu-id="fcad0-147">L’adresse n’a pas pu être envoyée au processus de validation.</span><span class="sxs-lookup"><span data-stu-id="fcad0-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="fcad0-148">Aucun</span><span class="sxs-lookup"><span data-stu-id="fcad0-148">None</span></span> |

<span data-ttu-id="fcad0-149">Les codes postaux des États-Unis retournent quatre chiffres supplémentaires + un trait d’union, par exemple 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="fcad0-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-150">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-150">Next steps</span></span>

- <span data-ttu-id="fcad0-151">Pour obtenir des instructions plus détaillées, consultez la documentation technique et les questions fréquemment posées dans le [groupe de partenaires dédié](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).</span><span class="sxs-lookup"><span data-stu-id="fcad0-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="fcad0-152">Préparez l’intégration des modifications à l’aide de l’API Espace partenaires et de l’expérience utilisateur web.</span><span class="sxs-lookup"><span data-stu-id="fcad0-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="fcad0-153">Partagez votre ID de locataire sandbox avec l’expert technique (Ali Khaki) afin de l’inclure dans la série de tests et de pouvoir commencer à préparer la mise à jour.</span><span class="sxs-lookup"><span data-stu-id="fcad0-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="fcad0-154">Si vous utilisez une solution de fournisseur de panneau de contrôle (CPV), consultez le fournisseur concerné.</span><span class="sxs-lookup"><span data-stu-id="fcad0-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-155">Des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-155">Questions?</span></span>

<span data-ttu-id="fcad0-156">Si vous avez besoin d’aide pour vos opérations Microsoft, contactez le groupe Yammer de votre support partenaire ou [faites une demande de service](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="fcad0-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="fcad0-157">Nouvel emplacement pour la documentation Swagger de l’API de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="fcad0-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-158">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-158">Categories</span></span>

- <span data-ttu-id="fcad0-159">Date : 26/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="fcad0-160">Fonctions</span><span class="sxs-lookup"><span data-stu-id="fcad0-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-161">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-161">Summary</span></span>

<span data-ttu-id="fcad0-162">Les documents Swagger de l’API Espace partenaires ont été déplacés de l’[ancien site de documentation Swagger](https://apidocs.microsoft.com/services/partnercenter) vers le [nouveau site de documentation Swagger](https://docs.microsoft.com/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="fcad0-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-163">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-163">Impacted audience</span></span>

<span data-ttu-id="fcad0-164">Les partenaires à facturation directe et les fournisseurs indirects participant au programme CSP qui utilisent les API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="fcad0-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-165">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-165">Details</span></span>

<span data-ttu-id="fcad0-166">À compter du 26 avril 2021, la documentation Swagger de l’API Espace partenaires, y compris le contenu de l’API REST, se trouve sur un [nouveau site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="fcad0-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="fcad0-167">L’ancien site deviendra inaccessible dans les semaines qui suivront.</span><span class="sxs-lookup"><span data-stu-id="fcad0-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="fcad0-168">Avantages</span><span class="sxs-lookup"><span data-stu-id="fcad0-168">Benefits</span></span>

<span data-ttu-id="fcad0-169">La documentation Swagger de l’API Espace partenaires fournit une **fonction d’essai**.</span><span class="sxs-lookup"><span data-stu-id="fcad0-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="fcad0-170">Pour utiliser cette fonction, vous devez disposer d’un jeton du porteur, que vous pouvez générer en suivant les étapes indiquées dans [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span><span class="sxs-lookup"><span data-stu-id="fcad0-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-171">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-171">Next steps</span></span>

<span data-ttu-id="fcad0-172">Partagez ces informations dans votre organisation pour permettre à l’équipe compétente de passer en revue et de mettre à jour ses processus.</span><span class="sxs-lookup"><span data-stu-id="fcad0-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-173">Vous avez des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-173">Questions?</span></span>

<span data-ttu-id="fcad0-174">Si vous avez des questions sur ces offres, consultez les communautés Yammer appropriées.</span><span class="sxs-lookup"><span data-stu-id="fcad0-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="fcad0-175">Politique de période de retour des logiciels de fournisseur de solutions Cloud (CSP) et avis d’expiration du lien de téléchargement</span><span class="sxs-lookup"><span data-stu-id="fcad0-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-176">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-176">Categories</span></span>

- <span data-ttu-id="fcad0-177">Date : 21/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="fcad0-178">Fonctions</span><span class="sxs-lookup"><span data-stu-id="fcad0-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-179">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-179">Summary</span></span>

<span data-ttu-id="fcad0-180">Des modifications ont été apportées à la politique concernant la période de retour des logiciels CSP et l’expiration du lien de téléchargement.</span><span class="sxs-lookup"><span data-stu-id="fcad0-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-181">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-181">Impacted audience</span></span>

<span data-ttu-id="fcad0-182">Partenaires proposant des offres d’abonnement à des logiciels avec licence perpétuelle ou non dans le programme CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-183">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-183">Details</span></span>

<span data-ttu-id="fcad0-184">Tenez compte des notifications importantes qui suivent concernant les achats d’abonnement à des logiciels avec licence perpétuelle ou non, via l’Espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="fcad0-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="fcad0-185">Politique relative à la période de retour des logiciels</span><span class="sxs-lookup"><span data-stu-id="fcad0-185">Software return period policy</span></span>

<span data-ttu-id="fcad0-186">Comme le stipule le Contrat Partenaire Microsoft (MPA), à partir du 1er juin 2021, la période de retour pour les offres logicielles dans le cadre du programme CSP passe de 60 jours à 30 jours à compter de la date de la commande.</span><span class="sxs-lookup"><span data-stu-id="fcad0-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="fcad0-187">Une fois qu’une commande a été effectuée pour une offre logicielle, les partenaires auront 30 jours à compter de la date de commande pour envoyer les révisions suivantes :</span><span class="sxs-lookup"><span data-stu-id="fcad0-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="fcad0-188">Toute licence perpétuelle de logiciel retournée pendant la période de retour de 30 jours fera l’objet d’un remboursement intégral du prix d’achat.</span><span class="sxs-lookup"><span data-stu-id="fcad0-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="fcad0-189">Tout abonnement à un produit logiciel retourné pendant la période de retour de 30 jours fera l’objet d’un remboursement calculé au prorata du prix d’achat.</span><span class="sxs-lookup"><span data-stu-id="fcad0-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="fcad0-190">Ce message fait suite aux e-mails que nous avons envoyés en décembre 2020 et en avril 2021 à tous les partenaires CSP, au sujet de la période de retour et d’autres informations sur le contrat MPA.</span><span class="sxs-lookup"><span data-stu-id="fcad0-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="fcad0-191">Reportez-vous à ces e-mails pour obtenir des informations complètes sur les modifications qui affectent le contrat MPA.</span><span class="sxs-lookup"><span data-stu-id="fcad0-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="fcad0-192">Expiration du lien de téléchargement de logiciel</span><span class="sxs-lookup"><span data-stu-id="fcad0-192">Software download link expiry</span></span>

<span data-ttu-id="fcad0-193">À compter du 3 juin 2021, les liens de téléchargement pour les abonnements à des logiciels avec licence perpétuelle ou non via l’Espace partenaires expireront au bout de cinq jours à compter du premier téléchargement.</span><span class="sxs-lookup"><span data-stu-id="fcad0-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="fcad0-194">La période d’expiration s’appliquera à tous les achats effectués avant le 3 juin 2021, ainsi que le 3 juin 2021 et après cette date.</span><span class="sxs-lookup"><span data-stu-id="fcad0-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-195">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-195">Next steps</span></span>

<span data-ttu-id="fcad0-196">Lisez les [Questions fréquentes relatives à la période de retour et à l’expiration du lien de téléchargement dans le programme CSP](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), et informez toutes les équipes concernées de votre organisation de ces modifications :</span><span class="sxs-lookup"><span data-stu-id="fcad0-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-197">Vous avez des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-197">Questions?</span></span>

<span data-ttu-id="fcad0-198">Si vous avez des questions sur ces offres, consultez les communautés Yammer appropriées.</span><span class="sxs-lookup"><span data-stu-id="fcad0-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="fcad0-199">Programme Open License : transition des revendeurs vers le programme Fournisseur de solutions Cloud (CSP)</span><span class="sxs-lookup"><span data-stu-id="fcad0-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-200">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-200">Categories</span></span>

- <span data-ttu-id="fcad0-201">Date : 19/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="fcad0-202">Développer votre activité</span><span class="sxs-lookup"><span data-stu-id="fcad0-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-203">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-203">Summary</span></span>

<span data-ttu-id="fcad0-204">Cette communication explique en détail comment se préparer aux changements qui seront bientôt apportés au programme Open License.</span><span class="sxs-lookup"><span data-stu-id="fcad0-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-205">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-205">Impacted audience</span></span>

<span data-ttu-id="fcad0-206">Partenaires CSP et Open License</span><span class="sxs-lookup"><span data-stu-id="fcad0-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-207">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-207">Details</span></span>

<span data-ttu-id="fcad0-208">En 2020, Microsoft a [annoncé](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) la diffusion prochaine de licences logicielles perpétuelles aux partenaires et clients par le biais du programme Fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="fcad0-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="fcad0-209">La première étape a été franchie en janvier 2021 avec la mise à disposition d’offres commerciales de logiciels perpétuels.</span><span class="sxs-lookup"><span data-stu-id="fcad0-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="fcad0-210">La prochaine étape clé aura lieu en juillet 2021, lorsque les offres du [secteur public](https://aka.ms/openlicensepublicsector) seront disponibles.</span><span class="sxs-lookup"><span data-stu-id="fcad0-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="fcad0-211">Nous avons également [communiqué](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) qu’à compter du 1er janvier 2022, aucun nouvel achat de licence logicielle ou renouvellement de Software Assurance ou de services en ligne ne pourra être effectué dans le cadre du programme Open License.</span><span class="sxs-lookup"><span data-stu-id="fcad0-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="fcad0-212">La transition des logiciels perpétuels vers le programme CSP dans la nouvelle expérience commerciale aidera les partenaires à offrir des solutions diversifiées et des services managés dans davantage de scénarios.</span><span class="sxs-lookup"><span data-stu-id="fcad0-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="fcad0-213">Cela accélèrera également la transition des clients vers le cloud.</span><span class="sxs-lookup"><span data-stu-id="fcad0-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="fcad0-214">Pour garantir une transition fluide à la fois pour nos partenaires et nos clients, nous avons effectué des ajustements et créé des documents visant à accélérer la transformation numérique :</span><span class="sxs-lookup"><span data-stu-id="fcad0-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="fcad0-215">Avril 2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-215">April 2021</span></span>

<span data-ttu-id="fcad0-216">[Disponible immédiatement](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/) : documents de transition Open License vers CSP pour les revendeurs</span><span class="sxs-lookup"><span data-stu-id="fcad0-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="fcad0-217">Juillet 2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="fcad0-218">CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-218">CSP</span></span>

- <span data-ttu-id="fcad0-219">1er juillet : Licences logicielles perpétuelles disponibles pour les clients du secteur public</span><span class="sxs-lookup"><span data-stu-id="fcad0-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="fcad0-220">7 juillet : Licences logicielles perpétuelles Visual Studio Pro et Get Genuine Windows Agreement disponibles pour tous les segments</span><span class="sxs-lookup"><span data-stu-id="fcad0-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="fcad0-221">Open Value</span><span class="sxs-lookup"><span data-stu-id="fcad0-221">Open Value</span></span>

- <span data-ttu-id="fcad0-222">1er juillet : Références SKU supplémentaires disponibles dans le programme Open Value pour l’éducation et les associations, avec des offres similaires à celles du programme Open License</span><span class="sxs-lookup"><span data-stu-id="fcad0-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="fcad0-223">Open License</span><span class="sxs-lookup"><span data-stu-id="fcad0-223">Open License</span></span>

- <span data-ttu-id="fcad0-224">1er juillet : Microsoft ne lancera plus de nouvelles offres dans le cadre du programme Open License.</span><span class="sxs-lookup"><span data-stu-id="fcad0-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="fcad0-225">Janvier 2022</span><span class="sxs-lookup"><span data-stu-id="fcad0-225">January 2022</span></span>

- <span data-ttu-id="fcad0-226">1er janvier : Aucun nouvel achat ou renouvellement ne pourra être effectué par le biais du programme Open License.</span><span class="sxs-lookup"><span data-stu-id="fcad0-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-227">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="fcad0-228">Fournisseurs indirects CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-228">CSP indirect providers</span></span>

<span data-ttu-id="fcad0-229">Profitez des mois à venir pour aider les revendeurs Open License à s’orienter vers le programme CSP en participant à des événements organisés par la communauté des partenaires et en utilisant les documents de transition Open License vers CSP pour les revendeurs :</span><span class="sxs-lookup"><span data-stu-id="fcad0-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="fcad0-230">[Documents de transition Open License vers CSP pour les revendeurs](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/) : présentation personnalisable, modèle d’e-mail, guide d’intégration des revendeurs indirects CSP, etc. pour encourager vos revendeurs à adopter le programme à grande échelle.</span><span class="sxs-lookup"><span data-stu-id="fcad0-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="fcad0-231">[Événements de la communauté des partenaires CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) organisés par Microsoft Business organisée.</span><span class="sxs-lookup"><span data-stu-id="fcad0-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="fcad0-232">Rejoignez les différentes sessions proposées pour apprendre les principes de base du programme CSP ou vous tenir à jour, et posez des questions sur les logiciels dans CSP (sessions de questions et réponses).</span><span class="sxs-lookup"><span data-stu-id="fcad0-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="fcad0-233">(Bientôt disponible) Session de formation destinée aux revendeurs indirects CSP organisée par Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="fcad0-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="fcad0-234">Revendeurs Open License</span><span class="sxs-lookup"><span data-stu-id="fcad0-234">Open License resellers</span></span>

- <span data-ttu-id="fcad0-235">Si votre organisation n’est pas actuellement inscrite au programme CSP, contactez votre distributeur pour savoir par où commencer.</span><span class="sxs-lookup"><span data-stu-id="fcad0-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="fcad0-236">Cliquez [ici](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider) pour contacter un fournisseur indirect.</span><span class="sxs-lookup"><span data-stu-id="fcad0-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="fcad0-237">Si votre organisation est déjà inscrite au programme CSP, cliquez [ici](https://partner.microsoft.com/resources/collection/software-in-csp) pour en savoir plus sur les logiciels perpétuels dans CSP.</span><span class="sxs-lookup"><span data-stu-id="fcad0-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-238">Vous avez des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-238">Questions?</span></span>

<span data-ttu-id="fcad0-239">Si vous avez d’autres questions sur ces offres, consultez vos communautés Yammer pertinentes.</span><span class="sxs-lookup"><span data-stu-id="fcad0-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="fcad0-240">Maintenant disponible : Guide de préparation des promotions mondiales</span><span class="sxs-lookup"><span data-stu-id="fcad0-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-241">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-241">Categories</span></span>

- <span data-ttu-id="fcad0-242">Date : 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="fcad0-243">Fonctions</span><span class="sxs-lookup"><span data-stu-id="fcad0-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-244">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-244">Summary</span></span>

<span data-ttu-id="fcad0-245">Launch Readiness a publié un nouveau [guide de préparation des promotions mondiales](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) dans la galerie de ressources Operations Readiness.</span><span class="sxs-lookup"><span data-stu-id="fcad0-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="fcad0-246">Ce guide offre une vue consolidée de toutes les [promotions actives à l’échelle mondiale](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span><span class="sxs-lookup"><span data-stu-id="fcad0-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-247">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-247">Impacted audience</span></span>

<span data-ttu-id="fcad0-248">Tous les partenaires VL (licence en volume), DPL (liste de prix Dynamics) et CSP (Fournisseur de solutions Cloud)</span><span class="sxs-lookup"><span data-stu-id="fcad0-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-249">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-249">Details</span></span>

<span data-ttu-id="fcad0-250">Les partenaires Microsoft nous ont fait part de la nécessité de disposer d’un guide regroupant toutes les promotions mondiales avec les détails de chaque offre.</span><span class="sxs-lookup"><span data-stu-id="fcad0-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="fcad0-251">Le but de ce guide est de regrouper toutes les informations disponibles dans un emplacement central et facilement accessible pour aider les partenaires à utiliser les promotions.</span><span class="sxs-lookup"><span data-stu-id="fcad0-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="fcad0-252">À compter d’avril 2021, Microsoft mettra à jour ce guide tous les mois et le publiera dans une collection de guides de préparation des promotions mondiales. Celle collection dédiée sera disponible dans la galerie de ressources Operations Readiness.</span><span class="sxs-lookup"><span data-stu-id="fcad0-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="fcad0-253">Des liens vers ce guide seront également inclus dans les collections suivantes :</span><span class="sxs-lookup"><span data-stu-id="fcad0-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="fcad0-254">La [collection de calendriers de lancement](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), qui fournit une vue centralisée des changements et des lancements à venir.</span><span class="sxs-lookup"><span data-stu-id="fcad0-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="fcad0-255">Les [collections de la communauté](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), qui contiennent des documents de support pour nos appels mensuels aux partenaires et qui soulignent les changements à venir et les sujets d’actualité présentant un intérêt opérationnel.</span><span class="sxs-lookup"><span data-stu-id="fcad0-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="fcad0-256">Les [bulletins d’informations pour les partenaires](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), notamment les mises à jour apportées chaque mois au programme CSP.</span><span class="sxs-lookup"><span data-stu-id="fcad0-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="fcad0-257">En guise de rappel, nous publierons également chaque mois une annonce dans l’Espace partenaires pour signaler la parution du nouveau numéro du guide de préparation des promotions mondiales.</span><span class="sxs-lookup"><span data-stu-id="fcad0-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-258">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-258">Next steps</span></span>

<span data-ttu-id="fcad0-259">Au début de chaque mois, vous trouverez le dernier [guide de préparation des promotions mondiales](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) dans la [galerie des ressources Operations Readiness](https://partner.microsoft.com/resources).</span><span class="sxs-lookup"><span data-stu-id="fcad0-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="fcad0-260">Partagez ces informations avec les personnes concernées dans vos organisations et donnez-nous votre avis sur le guide en utilisant le bouton « Cette page vous a-t-elle été utile ? »</span><span class="sxs-lookup"><span data-stu-id="fcad0-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="fcad0-261">à la fin de chaque page.</span><span class="sxs-lookup"><span data-stu-id="fcad0-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="fcad0-262">Mise à jour et rappels de la communauté pour les fournisseurs de solutions cloud (CSP) - Avril</span><span class="sxs-lookup"><span data-stu-id="fcad0-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-263">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-263">Categories</span></span>

- <span data-ttu-id="fcad0-264">Date : 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="fcad0-265">Communauté | Invitations et rappels</span><span class="sxs-lookup"><span data-stu-id="fcad0-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-266">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-266">Summary</span></span>

<span data-ttu-id="fcad0-267">Les ressources de la communauté CSP sont disponibles à la demande et mises à jour chaque mois pour vous tenir informé des changements apportés au programme CSP.</span><span class="sxs-lookup"><span data-stu-id="fcad0-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-268">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-268">Impacted audience</span></span>

<span data-ttu-id="fcad0-269">Partenaires à facturation directe et fournisseurs indirects inscrits à CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-270">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-270">Details</span></span>

<span data-ttu-id="fcad0-271">Ce mois-ci, les ressources incluent les sujets clés suivants :</span><span class="sxs-lookup"><span data-stu-id="fcad0-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="fcad0-272">Mise à jour de l’évolution du programme CSP et changements du programme Open License</span><span class="sxs-lookup"><span data-stu-id="fcad0-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="fcad0-273">Changements des conditions d’intégration des clients CSP dans certaines régions</span><span class="sxs-lookup"><span data-stu-id="fcad0-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="fcad0-274">Nouveau format de la nouvelle facture PDF commerciale dans le programme CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="fcad0-275">Dans la [collection de la communauté CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), vous trouverez :</span><span class="sxs-lookup"><span data-stu-id="fcad0-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="fcad0-276">Le [bulletin des mises à jour mensuelles du programme CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), qui regroupe les annonces récentes, mises à jour, événements et rappels en rapport avec le programme CSP dans un document convivial.</span><span class="sxs-lookup"><span data-stu-id="fcad0-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="fcad0-277">Le [calendrier des annonces CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), qui liste chronologiquement les changements à venir affectant le programme.</span><span class="sxs-lookup"><span data-stu-id="fcad0-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="fcad0-278">Le nouveau [calendrier de lancement de produit](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), dans lequel vous pouvez voir les lancements et les offres de produits à venir.</span><span class="sxs-lookup"><span data-stu-id="fcad0-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="fcad0-279">Les [ressources liées aux mises à jour apportées au programme CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/), avec du contenu facile à utiliser sur les changements opérationnels clés.</span><span class="sxs-lookup"><span data-stu-id="fcad0-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="fcad0-280">[Des sessions de recyclage et des rappels](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sur les principes clés du programme CSP suscitant de l’intérêt et des demandes.</span><span class="sxs-lookup"><span data-stu-id="fcad0-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="fcad0-281">Appel de la communauté CSP - Questions et réponses</span><span class="sxs-lookup"><span data-stu-id="fcad0-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="fcad0-282">Les questions et réponses des appels de la communauté sont disponibles pour vous aider à répondre à vos interrogations sur les changements à venir.</span><span class="sxs-lookup"><span data-stu-id="fcad0-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="fcad0-283">Inscrivez-vous dès à présent aux sessions de questions et réponses lors des appels de la communauté CSP qui auront lieu en avril, mai et juin.</span><span class="sxs-lookup"><span data-stu-id="fcad0-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="fcad0-284">Ces appels porteront sur les derniers lancements et fourniront des sessions de recyclage et des rappels importants.</span><span class="sxs-lookup"><span data-stu-id="fcad0-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="fcad0-285">[Inscrivez-vous ici](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span><span class="sxs-lookup"><span data-stu-id="fcad0-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-286">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-286">Next steps</span></span>

<span data-ttu-id="fcad0-287">Passez en revue les ressources de la communauté et inscrivez-vous aux questions et réponses des appels de la communauté.</span><span class="sxs-lookup"><span data-stu-id="fcad0-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="fcad0-288">Pour tirer le meilleur parti des questions et réponses des appels de la communauté, passez en revue le contenu de la communauté à la demande et envoyez vos questions 48 heures au maximum avant l’appel.</span><span class="sxs-lookup"><span data-stu-id="fcad0-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-289">Des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-289">Questions?</span></span>

<span data-ttu-id="fcad0-290">La session mensuelle de questions et réponses lors de l’appel de la communauté CSP est le meilleur endroit pour poser des questions sur les changements affectant le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="fcad0-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="fcad0-291">Chaque mois, passez en revue les documents et envoyez vos questions à l’avance afin que nous puissions orienter la session sur les sujets qui vous intéressent le plus.</span><span class="sxs-lookup"><span data-stu-id="fcad0-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="fcad0-292">Pour plus d’informations, contactez le [support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span><span class="sxs-lookup"><span data-stu-id="fcad0-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="fcad0-293">Dernier rappel : Dépréciation de la qualification GET le 6 mai 2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-294">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-294">Categories</span></span>

- <span data-ttu-id="fcad0-295">Date : 04/05/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="fcad0-296">Fonctions</span><span class="sxs-lookup"><span data-stu-id="fcad0-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-297">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-297">Impacted audience</span></span>

<span data-ttu-id="fcad0-298">Partenaires proposant des offres Éducation, Sans but lucratif et Cloud de la communauté du secteur public par le biais du programme Fournisseur de solutions Cloud avec l’API Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="fcad0-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-299">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-299">Details</span></span>

<span data-ttu-id="fcad0-300">Cette annonce est faite à la suite des [améliorations de l’Espace partenaires publiées en décembre](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span><span class="sxs-lookup"><span data-stu-id="fcad0-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="fcad0-301">Dans le cadre de cette version, de nouvelles API pour les qualifications GET et POST ont été déployées et, par conséquent, **la qualification GET existante sera mise hors service le 6 mai 2021**.</span><span class="sxs-lookup"><span data-stu-id="fcad0-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="fcad0-302">D’ici là, vous devrez passer aux nouvelles API POST de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="fcad0-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="fcad0-303">Les nouvelles API POST vous permettront d’acheter des offres Éducation, et les nouvelles API GET des offres préqualifiées Sans but lucratif et Cloud de la communauté du secteur public.</span><span class="sxs-lookup"><span data-stu-id="fcad0-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-304">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-304">Next steps</span></span>

- <span data-ttu-id="fcad0-305">Pour garantir une transition réussie et dans les temps, **faites la mise à jour vers les nouvelles API**.</span><span class="sxs-lookup"><span data-stu-id="fcad0-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="fcad0-306">**Passez en revue les nouveaux changements de l’API Espace partenaires et le guide correspondant** dans les ressources de préparation opérationnelle : [Améliorations du processus de validation des clients Éducation dans l’Espace partenaires](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span><span class="sxs-lookup"><span data-stu-id="fcad0-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="fcad0-307">Partagez ces informations avec les équipes appropriées au sein de votre organisation et avec vos revendeurs pour les aider à anticiper ces changements.</span><span class="sxs-lookup"><span data-stu-id="fcad0-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-308">Des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-308">Questions?</span></span>

<span data-ttu-id="fcad0-309">Pour toute question relative à cette notification, contactez le [support technique de l’Espace partenaires](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span><span class="sxs-lookup"><span data-stu-id="fcad0-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="fcad0-310">Journal des modifications</span><span class="sxs-lookup"><span data-stu-id="fcad0-310">Change log</span></span>

- <span data-ttu-id="fcad0-311">4 mai 2021 : Dernier rappel de la dépréciation à venir de la qualification GET</span><span class="sxs-lookup"><span data-stu-id="fcad0-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="fcad0-312">9 avril 2021 : Rappel de la dépréciation à venir de la qualification GET</span><span class="sxs-lookup"><span data-stu-id="fcad0-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="fcad0-313">Février : Plannings mis à jour pour la dépréciation des qualifications GET et PUT</span><span class="sxs-lookup"><span data-stu-id="fcad0-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="fcad0-314">Janvier : Rappel des dépréciations à venir des qualifications GET et PUT</span><span class="sxs-lookup"><span data-stu-id="fcad0-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="fcad0-315">Nouveau format pour la nouvelle facture PDF commerciale dans CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-316">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-316">Categories</span></span>

- <span data-ttu-id="fcad0-317">Date : 05/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="fcad0-318">Fonctions</span><span class="sxs-lookup"><span data-stu-id="fcad0-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-319">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-319">Summary</span></span>

<span data-ttu-id="fcad0-320">Microsoft introduit un nouveau format pour les factures PDF commerciales dans le programme CSP (Cloud Solution Provider) afin d’afficher les détails de facturation par détail du produit au lieu de la description de la référence SKU.</span><span class="sxs-lookup"><span data-stu-id="fcad0-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-321">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-321">Impacted audience</span></span>

<span data-ttu-id="fcad0-322">Partenaires effectuant des transactions via le programme CSP</span><span class="sxs-lookup"><span data-stu-id="fcad0-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-323">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-323">Details</span></span>

<span data-ttu-id="fcad0-324">À compter du mois de mai 2021, Microsoft présente un nouveau format pour les factures PDF commerciales dans le programme CSP afin d’afficher les détails de facturation par détail du produit au lieu de la description de la référence SKU.</span><span class="sxs-lookup"><span data-stu-id="fcad0-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="fcad0-325">Avec cette nouvelle mise à jour, nous allons regrouper les éléments de ligne par type de produit tout en affichant chaque produit sur une ligne individuelle.</span><span class="sxs-lookup"><span data-stu-id="fcad0-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="fcad0-326">Les partenaires remarqueront l’entrée en vigueur de ce changement dans leur facture du mois de mai pour la période de facturation comprise entre le 1er avril 2021 et le 30 avril 2021.</span><span class="sxs-lookup"><span data-stu-id="fcad0-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="fcad0-327">Les offres affectées sont Microsoft Azure Reserved Instance, les abonnements Azure (plan Azure) et la Place de marché.</span><span class="sxs-lookup"><span data-stu-id="fcad0-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="fcad0-328">Toutes les demandes de crédit-refacturation effectuées après la mise à jour du format de facture seront générées au nouveau format.</span><span class="sxs-lookup"><span data-stu-id="fcad0-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="fcad0-329">Avantages pour les partenaires</span><span class="sxs-lookup"><span data-stu-id="fcad0-329">Partner benefits</span></span>

<span data-ttu-id="fcad0-330">Cette mise à jour améliore l’expérience de facturation pour les partenaires des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="fcad0-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="fcad0-331">Réduction de la taille des factures tout en conservant les données critiques</span><span class="sxs-lookup"><span data-stu-id="fcad0-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="fcad0-332">Alignement du format sur les normes du secteur pour des factures compactes et conviviales</span><span class="sxs-lookup"><span data-stu-id="fcad0-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="fcad0-333">Les éléments suivants ne seront pas affectés :</span><span class="sxs-lookup"><span data-stu-id="fcad0-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="fcad0-334">Page de résumé de facturation sur le fichier PDF de facture</span><span class="sxs-lookup"><span data-stu-id="fcad0-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="fcad0-335">API de facturation existantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="fcad0-336">Fichiers de rapprochement (les fichiers de rapprochement peuvent être utilisés pour récupérer des données précises.)</span><span class="sxs-lookup"><span data-stu-id="fcad0-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="fcad0-337">Factures de frais d’utilisation et basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="fcad0-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-338">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-338">Next steps</span></span>

<span data-ttu-id="fcad0-339">Passez en revue les informations relatives à ce sujet dans la [galerie des ressources Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) sur le site web des partenaires Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcad0-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="fcad0-340">Pour plus d’informations sur la facturation et les taxes, notamment les ressources de facturation, les factures, la facturation des fournisseurs CSP et les taxes, consultez la [section Facturation](https://docs.microsoft.com/partner-center/billing) dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="fcad0-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="fcad0-341">Changements dans les conditions d’intégration des clients CSP (Cloud Solution Provider)</span><span class="sxs-lookup"><span data-stu-id="fcad0-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-342">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-342">Categories</span></span>

- <span data-ttu-id="fcad0-343">Date : 02/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="fcad0-344">Offres/marchés</span><span class="sxs-lookup"><span data-stu-id="fcad0-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="fcad0-345">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-345">Summary</span></span>

<span data-ttu-id="fcad0-346">Dans le cadre de notre engagement à aider les partenaires et les clients à exercer leur activité en toute confiance, nous demanderons des informations supplémentaires sur les clients à compter du 25 mars 2021.</span><span class="sxs-lookup"><span data-stu-id="fcad0-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-347">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-347">Impacted audience</span></span>

<span data-ttu-id="fcad0-348">Fournisseurs indirects et partenaires à facturation directe CSP qui ont des clients nouveaux ou existants dans les pays listés dans la section suivante</span><span class="sxs-lookup"><span data-stu-id="fcad0-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-349">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-349">Details</span></span>

<span data-ttu-id="fcad0-350">Chez Microsoft, la confiance est notre priorité.</span><span class="sxs-lookup"><span data-stu-id="fcad0-350">Microsoft runs on trust.</span></span> <span data-ttu-id="fcad0-351">Nous nous engageons à fournir une méthode de validation des clients conforme, sûre et sécurisée pour les transactions liées aux abonnements des clients dans le cadre du programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="fcad0-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="fcad0-352">Le 25 mars 2021, nous présenterons des améliorations de l’interface utilisateur et de l’API de l’Espace partenaires qui affecteront les partenaires répondant aux deux critères suivants :</span><span class="sxs-lookup"><span data-stu-id="fcad0-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="fcad0-353">Le partenaire a une relation de facturation directe avec Microsoft (ce qui signifie que le partenaire est un partenaire à facturation directe ou un fournisseur indirect).</span><span class="sxs-lookup"><span data-stu-id="fcad0-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="fcad0-354">Le partenaire fait affaire avec des clients nouveaux ou déjà existants dans les pays suivants :</span><span class="sxs-lookup"><span data-stu-id="fcad0-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="fcad0-355">Thaïlande</span><span class="sxs-lookup"><span data-stu-id="fcad0-355">Thailand</span></span>
    - <span data-ttu-id="fcad0-356">Vietnam</span><span class="sxs-lookup"><span data-stu-id="fcad0-356">Vietnam</span></span>
    - <span data-ttu-id="fcad0-357">Turquie</span><span class="sxs-lookup"><span data-stu-id="fcad0-357">Turkey</span></span>
    - <span data-ttu-id="fcad0-358">Pologne</span><span class="sxs-lookup"><span data-stu-id="fcad0-358">Poland</span></span>
    - <span data-ttu-id="fcad0-359">Afrique du Sud</span><span class="sxs-lookup"><span data-stu-id="fcad0-359">South Africa</span></span>
    - <span data-ttu-id="fcad0-360">Inde</span><span class="sxs-lookup"><span data-stu-id="fcad0-360">India</span></span>
    - <span data-ttu-id="fcad0-361">Brésil</span><span class="sxs-lookup"><span data-stu-id="fcad0-361">Brazil</span></span>
    - <span data-ttu-id="fcad0-362">Irak</span><span class="sxs-lookup"><span data-stu-id="fcad0-362">Iraq</span></span>
    - <span data-ttu-id="fcad0-363">Myanmar</span><span class="sxs-lookup"><span data-stu-id="fcad0-363">Myanmar</span></span>
    - <span data-ttu-id="fcad0-364">Soudan du Sud</span><span class="sxs-lookup"><span data-stu-id="fcad0-364">South Sudan</span></span>
    - <span data-ttu-id="fcad0-365">Arabie saoudite</span><span class="sxs-lookup"><span data-stu-id="fcad0-365">Saudi Arabia</span></span>
    - <span data-ttu-id="fcad0-366">Émirats arabes unis</span><span class="sxs-lookup"><span data-stu-id="fcad0-366">United Arab Emirates</span></span>
    - <span data-ttu-id="fcad0-367">Venezuela</span><span class="sxs-lookup"><span data-stu-id="fcad0-367">Venezuela</span></span>

<span data-ttu-id="fcad0-368">Les partenaires qui satisfont aux critères devront soumettre l’ID d’inscription d’entreprise d’un client (également connu sous le nom de code INN d’organisation) et le numéro de téléphone d’un client lors de la prochaine mise à jour ou création d’un abonnement pour ce client.</span><span class="sxs-lookup"><span data-stu-id="fcad0-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="fcad0-369">Ces partenaires peuvent également entrer un deuxième prénom facultatif pour le client.</span><span class="sxs-lookup"><span data-stu-id="fcad0-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="fcad0-370">Notez que lorsque vous ajoutez votre ID d’inscription d’entreprise, vous devez utiliser votre ID de taxe professionnelle et non l’ID personnel du client.</span><span class="sxs-lookup"><span data-stu-id="fcad0-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="fcad0-371">Les partenaires qui travaillent avec des clients nouveaux ou existants dans les pays suivants ont déjà été intégrés à une version précédente en novembre 2020.</span><span class="sxs-lookup"><span data-stu-id="fcad0-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="fcad0-372">Arménie</span><span class="sxs-lookup"><span data-stu-id="fcad0-372">Armenia</span></span>
- <span data-ttu-id="fcad0-373">Azerbaïdjan</span><span class="sxs-lookup"><span data-stu-id="fcad0-373">Azerbaijan</span></span>
- <span data-ttu-id="fcad0-374">Bélarus</span><span class="sxs-lookup"><span data-stu-id="fcad0-374">Belarus</span></span>
- <span data-ttu-id="fcad0-375">Hongrie</span><span class="sxs-lookup"><span data-stu-id="fcad0-375">Hungary</span></span>
- <span data-ttu-id="fcad0-376">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="fcad0-376">Kazakhstan</span></span>
- <span data-ttu-id="fcad0-377">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="fcad0-377">Kyrgyzstan</span></span>
- <span data-ttu-id="fcad0-378">Moldova</span><span class="sxs-lookup"><span data-stu-id="fcad0-378">Moldova</span></span>
- <span data-ttu-id="fcad0-379">Russie</span><span class="sxs-lookup"><span data-stu-id="fcad0-379">Russia</span></span>
- <span data-ttu-id="fcad0-380">Tadjikistan</span><span class="sxs-lookup"><span data-stu-id="fcad0-380">Tajikistan</span></span>
- <span data-ttu-id="fcad0-381">Ukraine</span><span class="sxs-lookup"><span data-stu-id="fcad0-381">Ukraine</span></span>
- <span data-ttu-id="fcad0-382">Ouzbékistan</span><span class="sxs-lookup"><span data-stu-id="fcad0-382">Uzbekistan</span></span>

<span data-ttu-id="fcad0-383">Les partenaires ayant des clients dans le reste du monde auront la possibilité à la fin du mois de mars 2021 d’entrer l’ID d’inscription d’entreprise, le numéro de téléphone et le deuxième prénom pour les clients, au titre d’informations facultatives.</span><span class="sxs-lookup"><span data-stu-id="fcad0-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-384">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-384">Next steps</span></span>

- <span data-ttu-id="fcad0-385">Pour obtenir des instructions plus détaillées, consultez la documentation technique et les questions fréquemment posées dans le [groupe de partenaires](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dédiée.</span><span class="sxs-lookup"><span data-stu-id="fcad0-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="fcad0-386">Préparez l’intégration des modifications à l’aide de l’API Espace partenaires et de l’expérience utilisateur web.</span><span class="sxs-lookup"><span data-stu-id="fcad0-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="fcad0-387">L’API et les SDK seront disponibles à des fins de test.</span><span class="sxs-lookup"><span data-stu-id="fcad0-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="fcad0-388">Veillez à soumettre les données supplémentaires lors de l’intégration de nouveaux clients ou de la modification des détails de clients existants.</span><span class="sxs-lookup"><span data-stu-id="fcad0-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="fcad0-389">Si vous utilisez une solution de fournisseur de panneau de contrôle (CPV), consultez le fournisseur concerné.</span><span class="sxs-lookup"><span data-stu-id="fcad0-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="fcad0-390">Des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-390">Questions?</span></span>

<span data-ttu-id="fcad0-391">Si vous avez des questions liées à l’ID d’inscription d’entreprise (également appelé code INN ou TIN), contactez votre conseiller fiscal ou le service des impôts local.</span><span class="sxs-lookup"><span data-stu-id="fcad0-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="fcad0-392">Microsoft ne peut pas fournir d’aide sur les questions fiscales.</span><span class="sxs-lookup"><span data-stu-id="fcad0-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="fcad0-393">Si vous avez besoin de support pour vos opérations avec Microsoft, [ouvrez une demande de service](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="fcad0-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="fcad0-394">Voir les lancements de produit et les offres du mois</span><span class="sxs-lookup"><span data-stu-id="fcad0-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="fcad0-395">Catégories</span><span class="sxs-lookup"><span data-stu-id="fcad0-395">Categories</span></span>

- <span data-ttu-id="fcad0-396">Date : 01/04/2021</span><span class="sxs-lookup"><span data-stu-id="fcad0-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="fcad0-397">Fonctions</span><span class="sxs-lookup"><span data-stu-id="fcad0-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="fcad0-398">Résumé</span><span class="sxs-lookup"><span data-stu-id="fcad0-398">Summary</span></span>

<span data-ttu-id="fcad0-399">Le calendrier de lancement de produit d’avril 2021 a été publié.</span><span class="sxs-lookup"><span data-stu-id="fcad0-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="fcad0-400">Public concerné</span><span class="sxs-lookup"><span data-stu-id="fcad0-400">Impacted audience</span></span>

<span data-ttu-id="fcad0-401">Tous les partenaires effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud</span><span class="sxs-lookup"><span data-stu-id="fcad0-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="fcad0-402">Détails</span><span class="sxs-lookup"><span data-stu-id="fcad0-402">Details</span></span>

<span data-ttu-id="fcad0-403">Le [calendrier de lancement de produit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) d’avril 2021 est maintenant disponible dans la galerie des ressources Operations readiness.</span><span class="sxs-lookup"><span data-stu-id="fcad0-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="fcad0-404">Vous pouvez y voir les lancements de produits et les offres à venir.</span><span class="sxs-lookup"><span data-stu-id="fcad0-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="fcad0-405">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcad0-405">Next steps</span></span>

<span data-ttu-id="fcad0-406">Passez en revue le [calendrier de lancement de produit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) et partagez les informations avec les parties prenantes appropriées de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="fcad0-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="fcad0-407">Vous avez des questions ?</span><span class="sxs-lookup"><span data-stu-id="fcad0-407">Questions?</span></span>

<span data-ttu-id="fcad0-408">Si vous avez d’autres questions sur ces offres, consultez vos communautés Yammer appropriées.</span><span class="sxs-lookup"><span data-stu-id="fcad0-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>
