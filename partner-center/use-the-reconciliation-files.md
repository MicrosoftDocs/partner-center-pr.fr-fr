---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 07/08/2019
description: Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 83be47cd9963d7e5f14b6c670cd57a8ab1d54011
ms.sourcegitcommit: 66afdaa662cfad217e29ba1f9e3a9ffd4349112f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/09/2019
ms.locfileid: "67694925"
---
# <a name="use-the-reconciliation-files"></a>Utiliser les fichiers de rapprochement

**S’applique à**

-  Espace partenaires
-  Espace partenaires de Microsoft Cloud for US Government


Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires. Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).

## <a name="formatting-issues"></a>Problèmes de mise en forme

Il peut arriver que votre fichier de rapprochement peut-être des problèmes de mise en forme. (Cela peut se produire, par exemple, si les paramètres régionaux EN-US ne sont pas utilisé.) Suivez les étapes ci-dessous pour résoudre ces problèmes. 

<ol>
<li>Ouvrez le fichier .csv dans Excel, puis sélectionnez la première colonne. Dans le ruban, sélectionnez <strong>données</strong>, puis sélectionnez <strong>texte aux colonnes</strong>.</li>

<li>Dans le texte de conversion Assistant, sélectionnez <strong>délimités de type de fichier</strong>, puis sélectionnez <strong>suivant</strong>.</li> 

<li>Dans le champ de séparateurs, sélectionnez <strong>virgules</strong>. Si <strong>onglet</strong> est déjà sélectionné, vous pouvez la laisser. Sélectionnez <strong>Suivant</strong>.</li>

<li>Dans le champ de format de données de colonne, sélectionnez <strong>Date : MDY</strong>, puis sélectionnez <strong>suivant</strong>.</li> 

<li>Dans le champ de format de données de colonne, sélectionnez <strong>texte</strong> pour tout montant de colonnes, puis sélectionnez <strong>Terminer</strong>.</li>
</ol>

## <a name="downloading-a-large-recon-file"></a>Téléchargement d’un fichier de rapprochement volumineux

Fichiers de rapprochement peuvent devenir très volumineux et sont parfois difficiles à télécharger. Pour un script PowerShell aider à télécharger de gros fichiers de rapprochement, consultez [Get facturation](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).

## <a href="" id="itemizebypartner"></a>Détailler par partenaire


Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licence pour détailler les informations par revendeur.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>ID&nbsp;MPN</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>ID&nbsp;MPN</td>
<td><p>L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</p></td>
</tr>
<tr class="even">
<td>ID&nbsp;MPN revendeur</td>
<td><p>Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</p>
<p>ID&nbsp;MPN du revendeur de référence pour l’abonnement. Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</p>
<p>vue d’eTo ou de mise à jour le revendeur, dans le menu espace partenaires, sélectionnez <strong>clients</strong>, puis sélectionnez le client dans la liste. Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste. Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</p>
<p>Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</p>
<p>Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</p>
<p>Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> Champs d’un fichier basé sur licence


Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Colonne</strong></td>
<td><strong>Description</strong></td>
<td><strong>Exemple de valeur</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>Identificateur unique de l’entité de facturation spécifique, au format GUID. Non requis pour le rapprochement, peut contenir des informations utiles. Identique dans toutes les lignes.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificateur unique pour une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</p>
<p>Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire. Voir Syndication_Partner_Subscription_Number.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>Syndication_Partner_Subscription_Number</td>
<td><p>Identificateur unique des abonnements. Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</p>
<p>Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>ID d’offre unique. ID d’offre standard conformément à la liste de prix.</p>
<p><b>Remarque</b>: Cette valeur ne correspond pas d’ID de l’offre à partir de la liste de prix. Voir DurableOfferID ci-dessous.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>ID d’offre unique durable, comme défini dans la liste des prix.</p>
<p><b>Remarque</b>: Cette valeur correspond à l’ID de l’offre à partir de la liste de prix.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</p></td>
<td>Microsoft Office 365 (Plan&nbsp;E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>La date de début d’abonnement, définie sur le jour suivant la soumission de la commande. En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</p>
<p>L’heure indique toujours le début de la journée, 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>La date de fin d’abonnement : 12 mois + x jours après la date de début (pour les aligner avec date de facturation du partenaire) ou 12 mois à partir de la date de renouvellement.</p>
<p>Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur. La communication avec les clients peut être nécessaire avant le renouvellement automatique.</p>
<p>L’heure indique toujours le début de la journée, 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>Date de début des frais.</p>
<p>Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</p>
<p>L’heure indique toujours le début de la journée, 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Jour de fin des frais.</p>
<p>Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</p>
<p>L’heure indique toujours la fin de la journée, 23:59.</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Le type de frais ou d’ajustement. Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></p></td>
<td><p>Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>Prix par siège, tel que publié dans la liste de prix au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantité</td>
<td><p>Nombre de sièges. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Montant</td>
<td><p>Prix total pour la quantité. Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Montant de la remise appliquée à ces frais. Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Sous-total</td>
<td><p>Total avant impôt. Vérifiez que le sous-total correspond au total prévu, en cas de remise.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Taxe</td>
<td><p>Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Total après impôts. Vérifie si les impôts sont retenus sur la facture.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>Type de devise. Chaque entité de facturation n’a qu’une devise. Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires. Cela est très important pour rapprocher la facture des informations de votre système.</p></td>
<td>Client test&nbsp;A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>ID&nbsp;MPN du partenaire&nbsp;CSP</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID&nbsp;MPN du revendeur de référence pour l’abonnement. Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Client&#39;-s nom de domaine, utilisé pour aider à identifier le client. Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365. Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</p></td>
<td>exemple.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>Pseudo d'abonnement. Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</p></td>
<td>PROJET EN LIGNE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. (Il s'agit d'un champ identique au nom Offre).</p></td>
<td>PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>Champs de fichier basée sur l’utilisation


Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.

Les champs suivants décrivent les services utilisés et leurs taux.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Colonne</strong></td>
<td><strong>Description</strong></td>
<td><strong>Exemple de valeur</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>ID partenaire au format GUID.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>Nom du partenaire.</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>ID de compte partenaire.</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires. Cela est très important pour rapprocher la facture des informations de votre système.</p></td>
<td>Client test&nbsp;A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>ID&nbsp;MPN du partenaire&nbsp;CSP.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID&nbsp;MPN du revendeur de référence pour l’abonnement. Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</p>
<p>L’heure indique toujours le début de la journée, 0:00.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</p>
<p>L’heure indique toujours la fin de la journée, 23:59.</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</p>
<p>Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>Pseudo de l’offre de service.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>Cœur de métier de l’offre de service</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificateur unique pour une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>Nom du service Azure en question.</p></td>
<td>MACHINES VIRTUELLES</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Type spécifique de service Windows&nbsp;Azure.</p></td>
<td><ul>
<li>Service Bus - Individuel ou Pack</li>
<li>Base de données SQL Azure - Entreprise ou Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Nom de ressource</td>
<td><p>Nom de la ressource Azure.</p></td>
<td><ul>
<li>Transfert de données entrantes (Go)</li>
<li>Transfert de données sortantes (Go)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Région</td>
<td><p>Région dans laquelle s’applique l’utilisation. Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</p></td>
<td>Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</td>
</tr>
<tr class="even">
<td>référence SKU</td>
<td><p>Identificateur unique MSFT de l’offre</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée. Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</p>
<p>Inclut également toute utilisation non facturée pour les périodes précédentes.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>Unités incluses dans le cadre de l’offre. Généralement non présent pour le programme Fournisseur de solutions Cloud.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</p>
<p>Correspond à ConsumedQuantity - IncludedQuantity.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>Prix de l’offre en vigueur à la date de début de l’abonnement.</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrist fois OverageQuantity, arrondi au centime près.</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Total après impôts, le cas échéant.</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>Type de devise. Chaque entité de facturation n’a qu’une devise. Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>Prix avant impôts par unité. Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>Prix après impôts par unité. Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Le type de frais ou d’ajustement. Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></p></td>
<td><p>Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>ID de compte unique dans la plateforme de facturation MSFT.</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>Date du déploiement du service.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</p></td>
<td>Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName. Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName. Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</p></td>
<td>AccessControl, CDN, Compute, Database, ServiceBus, Storage</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</p></td>
<td>EXTERNE</td>
</tr>
<tr class="even">
<td>Projet</td>
<td><p>Nom défini par le client pour son instance de service</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</p></td>
<td>Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ». Si vous aviez un pack de 25 connexions ServiceBus mis en service et vous aviez utilisé 1 pendant cette journée, votre relevé d’utilisation quotidienne pour ce jour indiquerait « 25 connexions / 30 jours – utilisé : 1.000000”.</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Client&#39;-s nom de domaine, utilisé pour aider à identifier le client. Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</p></td>
<td>exemple.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>Unit</td>
<td><p>Unité de la ressource.</p></td>
<td>Go ou heures</td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a>Champs de fichier uniques et récurrentes

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>colonne</th>
<th>Description</th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td>PartnerId</td>
<td><p>Identificateur de locataire Microsoft Azure Active Directory unique pour une entité de facturation spécifique, au format GUID. Non requis pour le rapprochement, peut contenir des informations utiles. Identique dans toutes les lignes.</p></td>
</tr>

<tr class="even">
<td>Id du client</td>
<td><p>Microsoft Azure Active Directory ID de locataire unique, au format GUID, utilisé pour identifier le client.</p></td>
</tr>

<tr class="odd">
<td>Nom du client</td>
<td><p>Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</p></td>
</tr>

<tr class="even">
<td>CustomerDomainName</td>
<td><p>Nom de domaine du client, afin d’identifier le client. Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365. Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</p></td>
</tr>

<tr class="odd">
<td>Pays du client</td>
<td><p>Le pays dans lequel se trouve le client.</p></td>
</tr>

<tr class="even">
<td>Numéro de facture</td>
<td><p>Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</p></td>
</tr>

<tr class="odd">
<td>MpnId</td>
<td><p>ID&nbsp;MPN du partenaire&nbsp;CSP.</p></td>
</tr>

<tr class="even">
<td>MpnId du revendeur</td>
<td><p>ID&nbsp;MPN du revendeur de référence pour l’abonnement.</p></td>
</tr>

<tr class="odd">
<td>ID de commande</td>
<td><p>Identificateur unique d’une commande dans la plateforme de commerce de Microsoft. Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</p></td>
</tr>

<tr class="even">
<td>Date de la commande</td>
<td><p>La date à laquelle la commande a été passée.</p></td>
</tr>

<tr class="odd">
<td>ProductId</td>
<td><p>ID du produit.</p></td>
</tr>

<tr class="even">
<td>SkuId</td>
<td><p>L’ID d'une référence SKU spécifique.</p></td>
</tr>

<tr class="odd">
<td>AvailabilityId</td>
<td><p>L’ID d'une disponibilité spécifique. La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</p></td>
</tr>

<tr class="even">
<td>Nom de la référence (SKU)</td>
<td><p>Le titre d'une référence spécifique.</p></td>
</tr>

<tr class="odd">
<td>Nom du produit</td>
<td><p>Le nom du produit.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>Nom du serveur de publication du produit.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>ID unique pour ce serveur de publication.</p></td>
</tr>

<tr class="even">
<td>Description de l’abonnement</td>
<td><p>Nom convivial d’un abonnement.</p></td>
</tr>

<tr class="odd">
<td>ID d’abonnement</td>
<td><p>Identificateur unique pour un abonnement dans la plateforme de commerce de Microsoft. Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement. Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Date de début des frais. L’heure indique toujours le début de la journée, 0:00.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Jour de fin des frais. L’heure indique toujours la fin de la journée, 23:59.</p></td>
</tr>

<tr class="even">
<td>Terme et Billingcycle</td>
<td><p>La longueur de terme et d’un cycle de facturation pour l’achat. Par exemple, « 1 an, tous les mois. »</p></td>
</tr>

<tr class="odd">
<td>Type de facturation</td>
<td><p>Le type de frais ou d’ajustement.</p></td>
</tr>

<tr class="even">
<td>Prix unitaire</td>
<td><p>Le prix publié dans la liste de prix au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</p></td>
</tr>

<tr class="odd">
<td>Prix unitaire efficace</td>
<td><p>Le prix unitaire après ont apporté des ajustements.</p></td>
</tr>

<tr class="even">
<td>Quantité</td>
<td><p>Nombre d’unités. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</p></td>
</tr>

<tr class="odd">
<td>Type d’unité</td>
<td><p>Le type d’unité achetée.</p></td>
</tr>

<tr class="even">
<td>DiscountDetails</td>
<td><p>Explication sur les remises applicables.</p></td>
</tr>

<tr class="odd">
<td>Sous-total</td>
<td><p>Total avant impôt. Vérifiez que le sous-total correspond au total prévu, en cas de remise.</p></td>
</tr>

<tr class="even">
<td>Total des taxes</td>
<td><p>Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</p></td>
</tr>

<tr class="odd">
<td>Total</td>
<td><p>Total après impôts. Vérifie si les impôts sont retenus sur la facture.</p></td>
</tr>

<tr class="even">
<td>Currency</td>
<td><p>Type de devise. Chaque entité de facturation n’a qu’une devise. Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</p></td>
</tr>

<tr class="odd">
<td>AlternateID</td>
<td><p>Un autre identificateur pour un ID de commande.</p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a>Champs de fichier d’utilisation quotidienne-évalués


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>colonne</th>
<th>Description</th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td>PartnerId</td>
<td><p>ID partenaire au format GUID.</p></td>
</tr>

<tr class="even">
<td>PartnerName</td>
<td><p>Nom du partenaire.</p></td>
</tr>

<tr class="odd">
<td>CustomerId</td>
<td><p>ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</p></td>
</tr>

<tr class="even">
<td>CustomerCompanyName</td>
<td><p>Nom de l’entreprise du client comme indiqué dans l’Espace partenaires. Cela est très important pour rapprocher la facture des informations de votre système.</p></td>
</tr>

<tr class="odd">
<td>CustomerDomainName</td>
<td><p>Le nom de domaine du client. Non disponible pour l’activité en cours.</p></td>
</tr>

<tr class="even">
<td>Pays du client</td>
<td><p>Le pays dans lequel se trouve le client.</p></td>
</tr>

<tr class="odd">
<td>MPNID</td>
<td><p>ID&nbsp;MPN du partenaire&nbsp;CSP.</p></td>
</tr>

<tr class="even">
<td>Revendeur MPNID</td>
<td><p>ID&nbsp;MPN du revendeur de référence pour l’abonnement. Non disponible pour l’activité en cours.</p></td>
</tr>

<tr class="odd">
<td>InvoiceNumber</td>
<td><p>Le numéro de la facture dans laquelle la transaction spécifiée apparaît. Non disponible pour l’activité en cours.</p></td>
</tr>

<tr class="even">
<td>ProductId</td>
<td><p>ID du produit.</p></td>
</tr>

<tr class="odd">
<td>SkuId</td>
<td><p>L’ID d'une référence SKU spécifique.</p></td>
</tr>

<tr class="even">
<td>AvailabilityId</td>
<td><p>L’ID d'une disponibilité spécifique. La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</p></td>
</tr>

<tr class="odd">
<td>Nom de la référence (SKU)</td>
<td><p>Le titre d'une référence spécifique.</p></td>
</tr>

<tr class="even">
<td>PublisherName</td>
<td><p>Le nom du serveur de publication.</p></td>
</tr>

<tr class="odd">
<td>PublisherID</td>
<td><p>L’ID du serveur de publication, au format GUID. Non disponible pour l’activité en cours.</p></td>
</tr>

<tr class=”even">
<td>Description de l’abonnement</td>
<td><p>Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. (Il s'agit d'un champ identique au nom Offre).</p></td>
</tr>

<tr class="odd">
<td>ID d’abonnement</td>
<td><p>Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement. Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</p></td>
</tr>

<tr class="even">
<td>ChargeStartDate</td>
<td><p>Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent). L’heure indique toujours le début de la journée, 0:00.</p></td>
</tr>

<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent). L’heure indique toujours la fin de la journée, 23:59.</p></td>
</tr>

<tr class="even">
<td>Date d’utilisation</td>
<td><p>Date de l’utilisation du service.</p></td>
</tr>

<tr class="odd">
<td>Type de compteur</td>
<td><p>Le type de compteur.</p></td>
</tr>

<tr class="even">
<td>Catégorie du compteur</td>
<td><p>Le service de niveau supérieur pour l’utilisation.</p></td>
</tr>

<tr class="odd">
<td>Id de compteur</td>
<td><p>L’ID du compteur utilisé.</p></td>
</tr>

<tr class="even">
<td>Sous-catégorie du compteur</td>
<td><p>Le type de service Azure qui peut affecter le tarif.</p></td>
</tr>

<tr class="odd">
<td>Nom du compteur</td>
<td><p>L’unité de mesure du compteur consommé.</p></td>
</tr>

<tr class="even">
<td>Région du compteur</td>
<td><p>Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</p></td>
</tr>

<tr class="odd">
<td>Unit</td>
<td><p>L’unité de la ressource de nom.</p></td>
</tr>

<tr class="even">
<td>Quantité consommée</td>
<td><p>Quantité de service utilisé (heures, Go, etc.) pendant la période en question. Inclut également toute utilisation non facturée pour les périodes précédentes.</p></td>
</tr>

<tr class="odd">
<td>Emplacement de la ressource</td>
<td><p>Le centre de données où le compteur est en cours d’exécution.</p></td>
</tr>

<tr class="even">
<td>Service consommé</td>
<td><p>Le service de plateforme Azure que vous avez utilisé.</p></td>
</tr>


<tr class="even">
<td>URI de ressource</td>
<td><p>L’URI de la ressource qui est utilisée.</p></td>
</tr>

<tr class="odd">
<td>Type de frais</td>
<td><p>Le type de frais ou d’ajustement. Non disponible pour l’activité en cours.</p></td>
</tr>

<tr class="even">
<td>Prix unitaire</td>
<td><p>Prix par licence, telles que publiées dans la liste de prix au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</p></td>
</tr>

<tr class="odd">
<td>Quantité</td>
<td><p>Nombre de licences. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</p></td>
</tr>

<tr class="even">
<td>Type d’unité</td>
<td><p>Le type d’unité dans que le compteur est facturé. Non disponible pour l’activité en cours.</p></td>
</tr>

<tr class="odd">
<td>Facturation avant impôts</td>
<td><p>Quantité totale avant impôts.</p></td>
</tr>

<tr class="even">
<td>Devise de facturation</td>
<td><p>La devise dans la région géographique du client</p></td>
</tr>

<tr class="odd">
<td>Prix total avant impôt</td>
<td><p>La tarification avant les taxes sont ajoutées.</p></td>
</tr>

<tr class="even">
<td>Tarification de devise</td>
<td><p>La devise dans la liste de prix.</p></td>
</tr>

<tr class="odd">
<td>Informations sur le service 1</td>
<td><p>Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</p></td>
</tr>

<tr class="even">
<td>Informations sur le service 2</td>
<td><p>Champ hérité capturant les métadonnées facultatives propres au service.</p></td>
</tr>

<tr class="even">
<td>Informations supplémentaires</td>
<td><p>Toute information supplémentaire non couverte dans d’autres colonnes.</p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a>Frais de mappage entre une facture et le fichier de réconciliation

Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.

Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.

Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés). Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’« ajustements » ne sont pas affichés dans le fichier de rapprochement.

Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement. 

<table>
<tbody>
<tr>
<td>
<p><strong>Description des frais de facture</strong></p>
</td>
<td>
<p><strong>Description des frais fichier de réconciliation (colonne ChargeType)</strong></p>
</td>
<td>
<p><strong>Qu’est ce coût ?</strong></p>
</td>
<td>
<p><strong>Comment pour mapper ces ChargeTypes à la facture ?</strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong>Frais sous licence</strong></p>
</td>
<td>
<p>Frais d'activation</p>
</td>
<td>
<p>Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</p>
</td>
<td rowspan="10">
<p>Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></p>
</td>
</tr>
<tr>
<td>
<p>Frais d'annulation</p>
</td>
<td>
<p>Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</p>
</td>
</tr>
<tr>
<td>
<p>Frais de cycle</p>
</td>
<td>
<p>Frais périodiques de l’abonnement</p>
</td>
</tr>
<tr>
<td>
<p>Instance de cycle au prorata</p>
</td>
<td>
<p>Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</p>
</td>
</tr>
<tr>
<td>
<p>Frais au prorata en cas d'annulation</p>
</td>
<td>
<p>Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</p>
</td>
</tr>
<tr>
<td>
<p>Frais au prorata à l'achat</p>
</td>
<td>
<p>Le type de frais pour un abonnement lors de l’utilisation de facturation annuelle</p>
</td>
</tr>
<tr>
<td>
<p>Frais d’abonnement</p>
</td>
<td>
<p>Le type de frais pour un abonnement lors de l’utilisation de la facturation mensuelle</p>
</td>
</tr>
<tr>
<td>
<p>Frais au prorata lors du renouvellement</p>
</td>
<td>
<p>Frais au prorata lors du renouvellement de l’abonnement</p>
</td>
</tr>
<tr>

<td>
<p>Frais de renouvellement</p>
</td>
<td>
<p>Frais de renouvellement d'un abonnement</p>
</td>
</tr>
<tr>
<td>
<p>Frais au prorata lors de l'activation</p>
</td>
<td>
<p>Frais au prorata de l’activation à la fin de la période de facturation</p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><strong>Frais à usage unique</strong></p>

</td>
<td>
<p>Nouveau</p>
</td>
<td>
<p>Utilisé lors de l’achat d’un nouveau est créé.</p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p>addQuantity</p>
</td>
<td>
<p>Utilisé dans les deux la restitution de l’achat d’origine et la quantité de nouveau après augmentation</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>removeQuantity</p>
</td>
<td>
<p>Utilisé dans les deux la restitution de l’achat d’origine et la quantité de nouveau après réduction</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Cancel</p>
</td>
<td>
<p>Utilisé quand un abonnement est annulé.</p>
</td>
</tr>

</tr>
<tr>
<td>
<p>Convertir</p>
</td>
<td>
<p>Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé</p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><strong>Frais d’utilisation</strong></p>
</td>
<td>
<p>Évaluer les frais d’utilisation lors de l'annulation</p>
</td>
<td>
<p>Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</p>
</td>
<td rowspan="2">
<p>À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Évaluer les frais d’utilisation pour le cycle actuel</p>
</td>
<td>
<p>Frais d’utilisation de l’accès pour la période de facturation en cours</p>
</td>
</tr>

<tr>
<td>
<p><strong>Crédits</strong></p>
</td>
<td>
<p>Décalage d’un élément de ligne</p>
</td>
<td>
<p>Remboursement partiel ou total d'un élément de ligne, taxes incluses</p>
</td>
<td>
<p>Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></p>
<p>À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong>Basée sur l’utilisation des remises</strong></p>
</td>
<td>
<p>Remise sur l’activation</p>
</td>
<td>
<p>Remise appliquée lors de l’activation de l’abonnement</p>
</td>

<td rowspan="4">
<p>À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Remise sur le cycle</p>
</td>
<td>
<p>Remise appliquée sur les frais périodiques</p>
</td>
</tr>
<tr>
<td>
<p>Renouveler la remise</p>
</td>
<td>
<p>Remise appliquée lors du renouvellement de l’abonnement</p>
</td>
</tr>
<tr>
<td>
<p>Annuler la remise</p>
</td>
<td>
<p>Frais appliqués lors de l’annulation des remises</p>
</td>
</tr>


<tr>
<td>
<p><strong>Remises sous licence</strong></p>
</td>
<td>
<p><em>Peut être appliqué à plusieurs types de frais</em></p>
</td>
<td>
<p></p>
</td>
<td>
<p>Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>Taxes</strong>  &nbsp;ou&nbsp;<strong>TVA</strong></p>
</td>
<td>
<p><em>Peut être appliqué à plusieurs types de frais</em></p>
<p><em>Exception : &quot;Compense un élément de ligne&quot; inclut déjà des taxes. Consultez des crédits, ci-dessus.</em></p>
</td>
<td>
<p>Taxes ou taxe sur la valeur ajoutée (TVA)</p>
</td>
<td>
<p>Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></p>
<p>À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
