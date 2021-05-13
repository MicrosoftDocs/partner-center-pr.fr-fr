---
title: Créer une association de clients
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Créer des associations de clients avec le modèle d’enregistrement (CPOR) du partenaire demandeur. Permet de gérer les ventes, l’utilisation, les Incentives pour Microsoft 365 & les clients Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856098"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="81cef-104">Associations de clients via le modèle CPOR (Partner of record) revendiqué pour Microsoft 365 et Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="81cef-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="81cef-105">**Rôles appropriés**: administrateur d’incentives</span><span class="sxs-lookup"><span data-stu-id="81cef-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="81cef-106">Le 1er octobre 2019, Microsoft a commencé à utiliser le modèle d’enregistrement (CPOR) du partenaire demandeur pour gérer les associations que vous avez avec votre Microsoft 365 et les clients Dynamics 365 en ce qui concerne la vente OSA (Online Services Advisory), l’utilisation des services en ligne (OSU)-Microsoft 365 et OSU-Business incentives sur les applications.</span><span class="sxs-lookup"><span data-stu-id="81cef-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="81cef-107">Les revendications de l’Association client (CPOR) s’appliquent uniquement à la vente des services de Conseil en ligne (OSA), à l’utilisation des services en ligne (OSU)-Microsoft 365 et aux programmes d’incentives des applications OSU-Business.</span><span class="sxs-lookup"><span data-stu-id="81cef-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="81cef-108">Si vous soumettez une demande de remboursement pour un autre programme, tel que le fournisseur de solutions Cloud, le revendeur géré, l’hébergement ou la surface, reportez-vous à la procédure décrite ici.</span><span class="sxs-lookup"><span data-stu-id="81cef-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="81cef-109">Lorsque vous soumettez votre revendication, Microsoft la valide.</span><span class="sxs-lookup"><span data-stu-id="81cef-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="81cef-110">Nous vous demanderons peut-être d’autres informations à ce stade.</span><span class="sxs-lookup"><span data-stu-id="81cef-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="81cef-111">Nous informerons également le client de votre demande d’association.</span><span class="sxs-lookup"><span data-stu-id="81cef-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="81cef-112">Les clients disposent de cinq jours ouvrés pour s’abonner. S’ils n’ont pas été refusés, votre association avec ce locataire et cette charge de travail spécifiques sera officielle.</span><span class="sxs-lookup"><span data-stu-id="81cef-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="81cef-113">À ce stade, vous aurez accès aux données d’utilisation du client.</span><span class="sxs-lookup"><span data-stu-id="81cef-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="81cef-114">Vous aurez besoin des informations suivantes pour effectuer une revendication :</span><span class="sxs-lookup"><span data-stu-id="81cef-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="81cef-115">**ID MPN** de votre entité qui effectue la revendication</span><span class="sxs-lookup"><span data-stu-id="81cef-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="81cef-116">Nom de **domaine** du client [Rechercher ce](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="81cef-116">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="81cef-117">ID de **répertoire** ou **ID de locataire** du client [Rechercher ce](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="81cef-117">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="81cef-118">La **zone** de la solution, telle que Business Applications ou Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="81cef-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="81cef-119">L' **activité** que vous avez effectuée et le type de revendication que vous souhaitez effectuer, telles que l’Association de pré-vente, d’utilisation ou de chiffre d’affaires</span><span class="sxs-lookup"><span data-stu-id="81cef-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="81cef-120">Le nom du **contact**, le titre et l’adresse de messagerie de votre client</span><span class="sxs-lookup"><span data-stu-id="81cef-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="81cef-121">Pour Dynamics 365, vous devez également fournir le nom, le titre et l’adresse de messagerie du **contact technique** de votre client.</span><span class="sxs-lookup"><span data-stu-id="81cef-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="81cef-122">Le **nom du contact** et l’adresse de messagerie de votre société</span><span class="sxs-lookup"><span data-stu-id="81cef-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="81cef-123">Vous allez créer un **nom** pour cette revendication.</span><span class="sxs-lookup"><span data-stu-id="81cef-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="81cef-124">**Produit (s)** ou charge (s) de travail que vous demandez</span><span class="sxs-lookup"><span data-stu-id="81cef-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="81cef-125">**Preuve d’exécution (PoE)**, telle qu’une déclaration de travail signée par le client.</span><span class="sxs-lookup"><span data-stu-id="81cef-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="81cef-126">Vous pouvez également télécharger un modèle PoE à utiliser.</span><span class="sxs-lookup"><span data-stu-id="81cef-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="81cef-127">Pour les partenaires revendiquant l’Association du chiffre d’affaires uniquement : **Dynamics solution seller Name**, **Customer Name** et **Name of ISV Product/solution**.</span><span class="sxs-lookup"><span data-stu-id="81cef-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="81cef-128">Vous devez également comprendre les points suivants :</span><span class="sxs-lookup"><span data-stu-id="81cef-128">You should also understand the following points:</span></span>

- <span data-ttu-id="81cef-129">Si vous avez des clients Microsoft 365 existants, vous devez réassocier à ceux pour lesquels vous souhaitez continuer à gagner des incentives OSU à l’aide de ce processus.</span><span class="sxs-lookup"><span data-stu-id="81cef-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="81cef-130">Si vous avez des associations existantes avec des clients Dynamics 365 ou Power BI, ces associations resteront valides jusqu’à l’expiration de leurs abonnements.</span><span class="sxs-lookup"><span data-stu-id="81cef-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="81cef-131">Un client peut avoir plusieurs partenaires, mais chaque charge de travail (pour OSU-Microsoft 365) ou abonnement (pour les applications OSA-Sell et OSU-Business) ne peut être associé qu’à un seul partenaire.</span><span class="sxs-lookup"><span data-stu-id="81cef-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="81cef-132">Créer une association de clients</span><span class="sxs-lookup"><span data-stu-id="81cef-132">Create a customer association</span></span>

1. <span data-ttu-id="81cef-133">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="81cef-133">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="81cef-134">Sélectionnez l’onglet **incentives** , sélectionnez **vue d’ensemble**, puis **associations client**.</span><span class="sxs-lookup"><span data-stu-id="81cef-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="81cef-135">En haut de la page des associations de clients, sélectionnez **+ Association client**.</span><span class="sxs-lookup"><span data-stu-id="81cef-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="81cef-136">Sélectionnez l’**ID MPN** du site partenaire à associer au client, puis ajoutez le nom du domaine et l’ID d’annuaire du client.</span><span class="sxs-lookup"><span data-stu-id="81cef-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="81cef-137">Rechercher</span><span class="sxs-lookup"><span data-stu-id="81cef-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="81cef-138">Sélectionnez **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="81cef-138">Select **Continue**.</span></span>

6. <span data-ttu-id="81cef-139">Sélectionnez la **zone de solution** et l' **activité**.</span><span class="sxs-lookup"><span data-stu-id="81cef-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="81cef-140">Si vous sélectionnez Business Applications, sélectionnez **utilisation et/ou prévente**, ou association de **chiffre d’affaires**, puis sélectionnez **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="81cef-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="81cef-141">Si vous sélectionnez Revenue association, vous serez invité à fournir des informations légèrement différentes de celles indiquées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="81cef-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="81cef-142">Entrez les informations appropriées dans la page **associer un client** , puis sélectionnez **créer une revendication**.</span><span class="sxs-lookup"><span data-stu-id="81cef-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="81cef-143">Sélectionnez le ou les produits associés à cette association de clients, puis sélectionnez **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="81cef-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="81cef-144">Renseignez les informations de contact du client, ainsi que les coordonnées de votre société.</span><span class="sxs-lookup"><span data-stu-id="81cef-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="81cef-145">Tous les champs sont obligatoires.</span><span class="sxs-lookup"><span data-stu-id="81cef-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="81cef-146">Si votre produit est Dynamics 365 et que le produit que vous choisissez a plusieurs abonnements pour ce client particulier, vous devez également entrer l’ID d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="81cef-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="81cef-147">Fournissez votre preuve d’exécution (PoE).</span><span class="sxs-lookup"><span data-stu-id="81cef-147">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="81cef-148">Vous pouvez la faire glisser vers la zone prévue, accéder à votre propre documentation de support ou utiliser un modèle en sélectionnant **Download template** (Télécharger un modèle).</span><span class="sxs-lookup"><span data-stu-id="81cef-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="81cef-149">Ajoutez puis enregistrez des commentaires si vous le souhaitez, puis sélectionnez **Submit claim** (Envoyer une demande).</span><span class="sxs-lookup"><span data-stu-id="81cef-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="81cef-150">Nous enverrons un e-mail au client qui demande l’approbation de votre association client.</span><span class="sxs-lookup"><span data-stu-id="81cef-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="81cef-151">Une fois que vous avez envoyé votre association client, vous ne pouvez plus la modifier.</span><span class="sxs-lookup"><span data-stu-id="81cef-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="81cef-152">L’état de votre association client s’affiche dans le champ **Status** (État).</span><span class="sxs-lookup"><span data-stu-id="81cef-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="81cef-153">Sélectionnez **History** (Historique) pour afficher l’historique d’une association client.</span><span class="sxs-lookup"><span data-stu-id="81cef-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="81cef-154">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="81cef-154">Next steps</span></span>

- [<span data-ttu-id="81cef-155">Gérer les associations client</span><span class="sxs-lookup"><span data-stu-id="81cef-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)