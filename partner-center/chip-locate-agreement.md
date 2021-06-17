---
title: Rechercher le nombre de postes de travail et le niveau de frais
ms.topic: how-to
ms.date: 02/18/2021
description: Découvrez comment utiliser la plateforme de revendeurs d’incentives pour rechercher le nombre de postes de travail et les informations de niveau de frais pour un accord.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276934"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Localiser le nombre de postes de travail et le niveau de frais pour un contrat

**Rôles appropriés**: contact principal ou administrateur de programme

Vous pouvez vous connecter à [explore.ms](https://www.explore.ms/) pour passer en revue le contrat ou télécharger un fichier fournissant les détails du contrat pour le nombre de postes de travail et le niveau de frais.

## <a name="to-locate-the-information"></a>Pour localiser les informations

### <a name="method-1--explorems"></a>Méthode 1 – Explore.ms

1. Ouvrez [explore.ms](https://www.explore.ms/) dans Internet Explorer. 

>[!Note]
>Vous ne pouvez pas exécuter cette fonction dans Google Chrome ou Microsoft Edge.

2. Connectez-vous avec votre compte professionnel ou scolaire ou Live ID.  

3. Dans le champ **rapports** , sélectionnez **contrats**.

4. Dans la page résultante, entrez le numéro de contrat dans le champ de **recherche** , puis sélectionnez **colonnes Select/Order**.

5. Dans la fenêtre contextuelle, sélectionnez le **nombre d’accords** dans la liste Colonnes disponibles, puis cliquez sur la flèche droite pour ajouter la colonne. Sélectionnez **OK**.

6. Sélectionnez **Rechercher.**

7. Dans l’écran qui s’affiche, faites défiler les résultats pour trouver la colonne **nombre d’ordinateurs** de l’accord. 

8. Utilisez le nombre de postes de travail pour déterminer le niveau de frais en fonction du tableau de taux ci-dessous.  

| Niveau de frais | Nombre de postes de travail |
| ------ | :-----------: |
|  Un | 0 – 2 399    |
|  B | 2 400 – 5 999    |
|  C | 6 000 – 14 999    |
|  D | 15000 +   |

>[!NOTE]
>Les niveaux d’incentives de l’entreprise sont basés sur le nombre d’utilisateurs ou de postes de travail (selon la valeur la plus élevée) des inscriptions au secteur commercial et public (PS). Pour les inscriptions sans nombre d’utilisateurs ou de postes de travail associés au niveau naturel, Microsoft applique un nombre de postes de travail en fonction du nombre de postes de travail ou du nombre d’utilisateurs de l’entreprise associée. <br><br>S’il n’y a pas d’accord associé, le niveau de prix est basé sur le niveau de tarification de l’inscription. Le niveau de tarification de la transaction peut également être consulté sur [www.explore.ms](https://www.explore.ms/). <br><br>S’il existe plusieurs niveaux de pool et/ou de tarification sur les contrats EA/EAS existants, Microsoft payera les incentives au niveau de la tarification/du pool affecté le plus élevé, le niveau A étant le plus bas et le niveau D étant le plus élevé.

#### <a name="pool-and-pricing-levels"></a>Niveaux de tarification et de pool

Après avoir effectué une recherche sur le numéro de contrat dans explore.ms à l’aide des étapes décrites ci-dessus, sélectionnez le numéro de contrat. Vous êtes alors sur la page Détails du contrat, qui affiche le récapitulatif et les **offres** de l' **accord** . La section offres contient les niveaux de tarification.

## <a name="method-2---chip"></a>Méthode 2-puce

1. Connectez-vous à la puce et sélectionnez les incentives LSP.

2. Dans la page **Résumé du paiement du partenaire** , sélectionnez le mois de rapport que vous souhaitez afficher, puis sélectionnez Détails du **calcul** dans la liste déroulante sous **Exporter vers Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Recherchez les détails du programme.":::

3. L’exportation démarre et vous pouvez ouvrir le fichier ou Enregistrer/Enregistrer sous dans une destination.

4. Lorsque le rapport est ouvert, accédez à l’onglet **DetailReport-FlatFile** en bas à gauche :

:::image type="content" source="images/chip/flatfile.png" alt-text="Téléchargement de fichier plat.":::

Vous pouvez maintenant rechercher le numéro de contrat que vous recherchez dans la colonne J. vous trouverez le nombre de postes de travail attribués dans la colonne R, étiqueté Agreement_DesktopCount. Vous pouvez également confirmer le niveau de frais pour ce contrat dans la colonne « AI » intitulée niveau.

## <a name="next-steps"></a>Étapes suivantes

- [Résoudre les problèmes d’accès au processeur](chip-access-trouble.md)
