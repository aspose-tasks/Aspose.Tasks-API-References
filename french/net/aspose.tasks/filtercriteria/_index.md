---
title: Class FilterCriteria
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.FilterCriteria classe. Définit les critères que les tâches ou les ressources doivent remplir pour être affichées dans la vue MSP.
type: docs
weight: 630
url: /fr/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Définit les critères que les tâches ou les ressources doivent remplir pour être affichées dans la vue MSP.

```csharp
public class FilterCriteria
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Obtient la liste des enfants`FilterCriteria` lignes. Si le filtre contient plus d'une ligne de critère, l'effet d'un opérateur Et est que les critères des deux lignes doivent être remplis pour que la tâche ou la ressource s'affiche à la suite de ce filtre. L'effet d'un Ou opérateur est que les critères pour l'une ou l'autre ligne doivent être remplis. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Obtient ou définit un[`Field`](./field/) changer. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Obtient ou définit le critère établi avec FieldName, Test et Value se rapporte à d'autres critères dans le filtre. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Obtient ou définit le type de comparaison effectuée entre FieldName et Value qui agit comme critère de sélection pour le filtre. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Obtient les valeurs d'objet à comparer avec la valeur du champ spécifié avec FieldName. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Renvoie la représentation sous forme de chaîne de l'instance du`FilterCriteria` classe. |

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)


