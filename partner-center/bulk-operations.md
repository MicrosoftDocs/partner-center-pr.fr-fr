---
title: Exporter et importer en bloc des opportunités de covente via des fichiers Excel/CSV dans des références
description: Découvrez comment télécharger, créer ou mettre à jour des opportunités de co-vente à l’aide de fichiers Excel (CSV) dans l’espace partenaires
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: c8910b98e32abe10ae3bc86f24aae7bec2630741
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880716"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Opérations en bloc pour les opportunités de co-vente à l’aide de fichiers de valeurs séparées par des virgules (CSV)

**Rôles appropriés**

- Administrateur des références
- Utilisateur Références

Les opérations en bloc dans l’espace partenaires permettent à l’entreprise d’exporter et d’importer des données d’opportunités de covente. Accédez à la page des **opportunités de covente** pour rechercher les liens **Importer** et **Exporter** en haut à droite de la bannière de titre de page. Les utilisateurs disposant des autorisations **administrateur** et **références utilisateur** peuvent utiliser cette fonctionnalité.

> [!IMPORTANT]
> Les actions de création/mise à jour effectuées par le biais d’une importation en bloc ne sont pas réversibles. Soyez prudent lorsque vous modifiez ou créez un grand nombre d’enregistrements. Seul un sous-ensemble de champs peut être modifié après la création d’une transaction. **Aucune action n’est autorisée une fois qu’une transaction atteint un état terminal comme refusé/expiré/gagné/perdu.**

## <a name="export-co-sell-opportunities"></a>Exporter les opportunités de covente

Les informations suivantes décrivent la fonctionnalité d’exportation :

- Vous pouvez exporter **jusqu’à 5000 enregistrements** en cliquant sur le bouton **Exporter** .
- Les contrats téléchargés seront basés sur vos niveaux d’accès. Les administrateurs de référence et les utilisateurs de référence peuvent obtenir des résultats différents en fonction de leur étendue et de leur inclusion en tant que membres de l’équipe dans le cadre des transactions. En savoir plus sur les [autorisations de références](permissions-overview.md#manage-referrals).
- La fonction d’exportation prend en compte l’onglet actuel dans la page opportunités de covente et les filtres qui ont été appliqués.
- Un fichier CSV contenant toutes les données basées sur les filtres appliqués sera généré.
- Le téléchargement des enregistrements peut prendre jusqu’à une minute.
- Vous n’avez pas besoin d’attendre la fin de l’action de téléchargement. Même si vous accédez à d’autres pages de l’espace partenaires, le fichier est téléchargé dès que la fonction d’exportation est terminée.
- Vous pouvez réutiliser le fichier téléchargé pour modifier les détails de la transaction et charger pour mettre à jour tous les enregistrements.

## <a name="import-co-sell-opportunities"></a>Importer des opportunités de covente

- Vous pouvez créer ou mettre à jour un **maximum de 1000 enregistrements** à l’aide de la fonctionnalité d’importation.
- Vous pouvez créer le modèle à partir de zéro en téléchargeant le modèle à partir de la page importer de l’espace partenaires.
- Vous pouvez également utiliser la fonctionnalité d’exportation pour télécharger les enregistrements existants et les mettre à jour.
- Si le fichier contient plus de 1000 enregistrements, il ne peut pas être traité.
- Une fois le fichier traité, un résumé indiquant le nombre de références qui ont été créées, mises à jour et non traitées s’affiche dans la dernière fiche de fichier de processus.
- Vous pouvez télécharger les détails des enregistrements traités, corriger les erreurs et télécharger le même fichier pour créer ou mettre à jour les enregistrements qui ont échoué lors de l’exécution précédente. **Supprimez tous les enregistrements réussis du fichier avant de télécharger les enregistrements corrigés qui ont échoué lors de l’exécution précédente.**
- Pour ajouter d’autres solutions, ajoutez des colonnes supplémentaires en regard de la solution 1 et utilisez le nom de colonne en tant que solution X, où X représente le numéro de la solution dans le contrat. Par exemple, solution 2, solution 3.
- Vous pouvez ajouter jusqu’à 50 solutions à un contrat.
- Pour ajouter d’autres membres de l’équipe, ajoutez des colonnes supplémentaires en regard de membre de l’équipe 1 et utilisez le nom de la colonne en tant que membre de l’équipe X, où X représente le numéro du membre de l’équipe dans le contrat. Par exemple, membre de l’équipe 2, membre de l’équipe 3.
- Vous pouvez ajouter jusqu’à 50 membres de l’équipe à un contrat.

> [!NOTE]
> Vous n’avez pas besoin d’attendre la fin du traitement. Les détails du dernier fichier traité seront disponibles en téléchargement une fois le traitement terminé. **L’opération peut prendre jusqu’à 10 minutes si vous téléchargez des fichiers avec des enregistrements 1000.**

> [!IMPORTANT]
> Lisez attentivement toutes les instructions et vérifiez le format de chaque colonne dans le tableau ci-dessous avant de créer ou de mettre à jour les transactions à l’aide de fichiers CSV dans l’espace partenaires.

|**Nom de la colonne**|**Est obligatoire ?**|**Description**|**Exemple de valeur (s)**|
|-----|:-----|:---------|:---|
Erreurs|Non|Les erreurs éventuelles liées aux opérations de création/mise à jour w. r. t pour les références seront incluses dans cette colonne. S’il y a plusieurs erreurs, elles sont toutes répertoriées en les séparant par un point-virgule.|La solution champ obligatoire 1 est manquante|
ID engagement|Non|L’ID engagement est généré par le système de références de l’espace partenaires Microsoft. Non requis pour la création d’une nouvelle référence. Vous pouvez utiliser l’ID d’engagement existant si vous mettez à jour un enregistrement.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
URL de référence|Non|L’ID de référence est généré par le système de références de l’espace partenaires Microsoft. Non requis pour la création d’une nouvelle référence. Remplissez-le avec l’ID de référence si vous mettez à jour un enregistrement existant.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nom de la transaction|Oui|Nom convivial pour le traitement de votre référence.|Contrat UK Printemps
Nom du client|Oui|Nom de la société cliente. Utilisez le nom légal de l’Organisation pour la correspondance rapide côté Microsoft.|Contoso Corporation
Adresse client, ligne 1|Oui|Adresse ligne 1 de la société du client. |Un moyen de contoso
Adresse client, ligne 2|Non|Adresse ligne 2 de la société du client.|Rue 148
Ville du client|Oui|Ville dans laquelle se trouve l’organisation cliente.|Redmond
État du client|Non|État où se trouve l’organisation cliente.|Washington
Code postal du client|Non|Code postal de la région où se trouve l’organisation cliente.|98052
Pays du client|Oui|Pays/région où se trouve l’organisation cliente. Utilisez les codes de pays à deux lettres comme indiqué [ici]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|US
ID du client D-U-N-S|Non|Essayez de récupérer l’ID DUNS de l’organisation cliente. Cela permet de faire correspondre plus rapidement l’organisation du client du côté Microsoft, ce qui permet une attribution plus rapide des vendeurs. Vous pouvez obtenir l’ID DUNS gratuitement à partir de ce [site Web](https://www.dnb.com/duns-number/lookup.html).|81466849
Prénom du contact client|Dépend|Le prénom est obligatoire uniquement si vous avez besoin de l’aide de Microsoft. Prénom du contact principal de l’organisation cliente qui travaille sur cette transaction.|John
Nom du contact du client|Dépend|Le nom est obligatoire uniquement si vous avez besoin de l’aide de Microsoft. Nom du contact principal de l’organisation cliente qui travaille sur cette transaction.|Client
Numéro de téléphone du contact client|Dépend|Le numéro de téléphone est obligatoire uniquement si vous avez besoin de l’aide de Microsoft. Numéro de téléphone du contact principal de l’organisation cliente qui travaille sur cette transaction.|9999999999
Adresse E-mail du contact client|Dépend|L’adresse de messagerie est obligatoire uniquement si vous avez besoin de l’aide de Microsoft. Adresse e-mail du contact principal de l’organisation cliente qui travaille sur cette transaction.|john.customer@contoso.com
État de la référence partenaire|Oui|Indique l’état de la transaction du point de vue de votre entreprise. Obligatoire si vous essayez de créer ou de modifier une référence. Utilisez **nouveau** si vous essayez de créer un nouveau contrat. Les valeurs acceptées sont documentées [ici](/partner/develop/referral-resources#referralstatus).|Actif
Sous-état de la référence du partenaire|Oui|Indique l’état exact de la transaction. Utilisez **accepté** si vous essayez de créer un nouveau contrat. Elle est également requise si vous modifiez une référence existante. Les valeurs acceptées sont documentées [ici](/partner/develop/referral-resources#referralsubstatus).|Accepté
État de la référence Microsoft|Dépend|Indique l’état de la demande de covente que vous avez envoyée à Microsoft pour rechercher de l’aide. Ce champ est en lecture seule. Toute modification apportée à ce champ lors de l’importation des données sera ignorée.| Pending
Raison refusée/perdue|Dépend| Vous devez fournir ces informations uniquement si vous modifiez le sous-état de votre champ pour qu’il soit refusé ou perdu. Sinon, vous pouvez ignorer cette colonne. <br/> **Entrez un nombre en fonction des options ci-dessous** <br/><br/> **1**-le budget du projet n’est pas adéquat  <br/> **2**-le client n’a pas répondu  <br/> **3**-le client a choisi un autre fournisseur  <br/> **4** -exigence du client non remplie  <br/> **5** -pas un client <br/> **6**-la chronologie proposée était trop petite <br/> **7** -signaler comme abus, courrier indésirable ou hameçonnage <br/> **8** -autres |6|
Étape de vente|Non|Il s’agit du champ pour indiquer l’étape détaillée des ventes de la référence. En savoir plus sur les étapes de vente [ici](./manage-co-sell-opportunities.md)|40
Estimation de la valeur de la transaction|Oui|Valeur de la transaction basée sur les conversations initiales avec le client. Cela peut être modifié jusqu’à ce que la transaction atteigne l’un des États terminal **gagnés** ou **perdus.**|12563
Devise|Oui|Devise dans laquelle la valeur de transaction est entrée. Vous trouverez [ici](https://en.wikipedia.org/wiki/ISO_4217)les codes de devise.|USD
Date de clôture estimée|Oui|Date de clôture estimée de la transaction en fonction des conversations initiales avec le client au format MM/jj/aaaa. <br/> **La date doit être le fuseau horaire UTC. Toutes les dates affichées dans l’interface utilisateur de l’espace partenaires sont basées sur les fuseaux horaires localisés. Il peut y avoir +/-une différence d’un jour dans l’interface utilisateur de l’espace partenaires si vous examinez la référence pour laquelle vous avez fourni la date au fuseau horaire UTC.**|1/30/2020
ID CRM|Non|Identificateur de cette référence spécifique dans votre système CRM, le cas échéant. Il s’agit d’un champ de saisie de texte de forme libre.|34234324-sdfsdf-345345-SFD
ID de campagne marketing|Non|Ce champ indique la campagne marketing, qui a abouti à cette référence spécifique. Généralement utilisé pour le calcul du ROI|BingSummer2020
Notes|Non|Remarques détaillées indiquant les mises à jour liées à la référence|Voici un exemple de note
Aide Microsoft requise ?|Oui|Cela permet d’indiquer si vous souhaitez que Microsoft vous aide à effectuer cette demande de co-vente|Oui
Quelle aide spécifique de Microsoft ?|Dépend|L’une des six différentes façons dont Microsoft peut vous aider. Cela s’applique uniquement si vous choisissez Oui pour la question «aide Microsoft requise ? " <br/> **Entrez un nombre en fonction des options ci-dessous** <br/><br/> **1**-proposition de valeur spécifique à la charge de travail  <br/> **2**-architecture technique client  <br/> **3**-preuve de concept/Demo  <br/> **4**-devis et licences  <br/> **5**: succès des clients après la vente  <br/> **6**-général ou autre|1|
Partager avec l’équipe de vente Microsoft|Oui|Cela permet d’indiquer si vous souhaitez partager les détails du contrat avec l’équipe de vente Microsoft. Cela s’applique uniquement si vous choisissez non pour la question «aide Microsoft requise ? "|Oui
Remarques à Microsoft|Non|Remarques spécifiques à Microsoft si vous avez besoin d’aide de Microsoft|Besoin d’aide avec un POC pour le client contoso
Consentement de partager le contact avec le client et le partenaire|Oui|Le consentement de partager les coordonnées du client et les informations de contact des employés de votre entreprise sont ceux qui travaillent sur la transaction. **Les transactions ne sont pas créées ou mises à jour si vous choisissez non pour cette colonne.** |Oui
Solution 1|Oui|ID de solution (obligatoire), devise (facultative) dans laquelle la valeur de transaction est entrée. Vous pouvez trouver les codes de devise [ici](https://en.wikipedia.org/wiki/ISO_4217), le prix de la référence (facultatif) et la quantité de la référence (facultatif).  |SOL-1234-PQRS, USD, 10, 100
Membre de l’équipe 1|Oui|Prénom, nom, numéro de téléphone portable et ID d’e-mail du membre de l’équipe respectif.| Bob, partenaire, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Étapes suivantes

Vous pouvez utiliser ces connecteurs de covente de l’espace partenaires pour vendre en collaboration avec Microsoft à partir de vos systèmes CRM.

- [Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble](connector-dynamics.md)
- [Connecteur de covente pour Salesforce CRM - vue d’ensemble](connector-salesforce.md)
