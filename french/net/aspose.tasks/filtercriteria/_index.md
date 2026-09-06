---
title: "Classe FilterCriteria"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.FilterCriteria. Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP."
type: docs
weight: 630
url: /fr/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Définit les critères que les tâches ou les ressources doivent satisfaire pour être affichés dans la vue MSP.

```csharp
public class FilterCriteria
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Obtient la liste des lignes enfants `FilterCriteria`. Si le filtre contient plus d'une ligne de critère, l'effet d'un opérateur ET est que les critères des deux lignes doivent être remplis pour que la tâche ou la ressource soit affichée en résultat de ce filtre. L'effet d'un opérateur OU est que les critères de l'une ou l'autre ligne doivent être remplis. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Obtient ou définit un [`Field`](./field/) à modifier. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Obtient ou définit le critère établi avec FieldName, Test et Value qui se rapporte aux autres critères du filtre. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Obtient ou définit le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour le filtre. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Obtient les valeurs d'objet à comparer avec la valeur du champ spécifié par FieldName. |

## Méthodes

| Nom | Description |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Obtient si la valeur à droite de FilterCriteria est une référence de champ, et non une valeur constante. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Définit le champ dont la valeur sera comparée à la valeur du champ spécifié par FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Renvoie la représentation sous forme de chaîne de l'instance de la classe `FilterCriteria`. |

## Exemples

Montre comment lire les critères de filtre de tâche.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// Imprimer les critères de filtre sous forme de chaîne 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


