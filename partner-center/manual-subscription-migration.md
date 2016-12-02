---
title: Migrer des abonnements Dynamics AX vers Dynamics365 | Espace partenaires
description: "Microsoft propose Dynamics365, la nouvelle génération d’applications métier intelligentes permettant à votre entreprise de se développer, croître et se transformer pour répondre aux besoins de vos clients et saisir de nouvelles opportunités."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 1d17213d3b591056d6af2dd1855d6c52a17801f5

---

# Migrer des abonnements Dynamics AX vers Dynamics365


Microsoft propose Dynamics365, la nouvelle génération d’applications métier intelligentes permettant à votre entreprise de se développer, croître et se transformer pour répondre aux besoins de vos clients et saisir de nouvelles opportunités. Dans le cadre du nouveau produit, Microsoft présente les nouvelles formules d’abonnement Microsoft Dynamics le 1ernovembre2016, qui sont similaires, mais pas identiques à vos formules actuelles.

Les instructions fournies dans ce document décrivent comment les fournisseurs indirects peuvent transformer les abonnements Microsoft DynamicsAX des clients en nouveaux abonnements Microsoft Dynamics365. Elles s’appliquent également aux autres produits Microsoft qui connaissent des mises à jour, obligeant les fournisseurs à migrer les abonnements des clients vers une nouvelle référence (SKU).

**Modifications des licences Microsoft DynamicsAX**

La gamme de produits Microsoft DynamicsAX n’est plus disponible à partir du 1ernovembre2016. Pour en savoir plus sur les nouvelles options de licence de Dynamics365, consultez le guide des licences qui sera bientôt publié. Pour plus d’informations sur le mappage de licences, consultez le tableau suivant:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Licence Dynamics AX retirée</strong></p></td>
<td><p><strong>Licence Dynamics 365</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Dynamics 365 Enterprise edition Plan 2</p>
<p>OR Dynamics 365 for Operations</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Task</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Functional</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Device</p></td>
<td><p>Dynamics 365 for Operations Device</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

La formule Microsoft Dynamics CRM Online actuelle n’est plus disponible depuis le 1ernovembre2016. Pour en savoir plus sur les nouvelles options de gestion de licences, consultez [Informations importantes pour les clients de CRM Online](https://go.microsoft.com/fwlink/?linkid=831667).

## Accompagner les clients vers les nouvelles formules de produit


Microsoft offre en permanence de nouveaux produits et services aux revendeurs et fournisseurs. Dans ces cas, un revendeur peut avoir besoin de mettre à niveau les services de ses clients ou de migrer leurs abonnements à partir de références (SKU) qui vont progressivement disparaître. La migration de clients depuis des références anciennes vers des références plus récentes doit respecter la séquence suivante:

-   [Acheter le nouvel abonnement](#manual-subscription-migration-purchasenewsubsc)
-   [Réaffecter les licences utilisateur actuelles](#manual-subscription-migration-reassignlicenses)
-   [Annuler l’ancien abonnement](#manual-subscription-migration-cancelsubscriptions)

Dans les procédures suivantes, vous migrez un client de Dynamics AX7 Enterprise vers Dynamics 365 for Operations.

<a href="" id="purchasenewsubsc"></a>
Le revendeur doit migrer un client avec un abonnement DynamicsAX Enterprise vers un abonnement Dynamics 365 for Operations. La première étape consiste à acheter Dynamics365 for Operations.

**Acheter le nouvel abonnement**

1.  Dans le menu **Tableau de bord**, sélectionnez **Clients** et le client à déplacer, puis choisissez **Ajouter des abonnements**.
2.  Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, Dynamics365 for Operations, Enterprise Edition), indiquez le nombre de licences et choisissez **Envoyer**.

    Votre client doit maintenant avoir un ancien et un nouvel abonnement: dans cet exemple, l’ancien (Dynamics AX Enterprise) et le nouveau (Dynamics365 for Operations, Enterprise Edition).

<a href="" id="reassignlicenses"></a>
L’étape suivante consiste à réaffecter toutes les licences utilisateur au nouvel abonnement.

**Réaffecter les licences utilisateur**

1.  Dans le menu **Tableau de bord**, sélectionnez **Clients** et le client à déplacer, puis choisissez **Utilisateurs et licences**. La page Utilisateurs et licences du client s’ouvre.
2.  Pour réaffecter les licences utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.
3.  Dans la page **Gérer les licences**, désactivez la case à cocher de la licence **Dynamics AX Enterprise**, puis sélectionnez la licence **Dynamics 365 for Operations**.
4.  Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées.
5.  Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.

<a href="" id="cancelsubscriptions"></a>
Une fois les licences utilisateur attribuées au nouveau service, vous pouvez en toute sécurité annuler l’ancien abonnement au premier niveau du client.

**Annuler l’ancien abonnement**

1.  Dans le menu **Tableau de bord**, sélectionnez **Clients** et le client à déplacer, puis choisissez l’abonnement à annuler.
2.  Dans la page de détails de l’abonnement, sélectionnez **Suspendu** dans **État**.
3.  Sélectionnez **Envoyer**.

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est automatiquement désapprovisionné après 120jours. Aucun frais n’est facturé au client pour l’ancien abonnement.

## Autres éléments à prendre en considération


Si votre client passe du programme Open Channel au programme Cloud Services pour approvisionner davantage d’abonnements, vous devrez également migrer ses abonnements:

-   Si le client a reçu son ancien abonnement via le programme Open Channel, la transition vers le programme Fournisseur de services Cloud sur la nouvelle référence (SKU) est simple.
-   Si le client n’est pas encore votre client, vous pouvez l’inviter. Pour plus d’informations, consultez la rubrique d’aide [Demander une relation avec un client](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Lorsque le client vous accepte comme fournisseur indirect, la procédure d’approvisionnement reste essentiellement la même: vous achetez le nouvel abonnement, puis vous affectez les licences utilisateur. La seule différence concerne l’annulation du ou des anciens abonnements. Un nouveau fournisseur ne peut pas annuler ou suspendre des abonnements souscrits par le biais d’autres canaux. Si le client a souscrit des abonnements via un autre canal de vente, comme le programme Open Channel, il doit les annuler lui-même dans ce canal.

 

 






<!--HONumber=Nov16_HO4-->


