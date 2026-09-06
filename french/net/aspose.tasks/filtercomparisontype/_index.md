---
title: "Enum FilterComparisonType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.FilterComparisonType enum. Le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour un filtre ou un indicateur graphique."
type: docs
weight: 620
url: /fr/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Le type de comparaison effectué entre FieldName et Value qui sert de critère de sélection pour un filtre ou un indicateur graphique.

```csharp
public enum FilterComparisonType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Equals | `6` | La valeur de Field est égale à Value. |
| DoesNotEqual | `7` | La valeur de Field n'est pas égale à Value. |
| IsGreaterThan | `2` | La valeur de Field est supérieure à Value. |
| IsGreaterThanOrEqualTo | `4` | La valeur de Field est supérieure ou égale à Value. |
| IsLessThan | `3` | La valeur de Field est inférieure à Value. |
| IsLessThanOrEqualTo | `5` | La valeur de Field est inférieure ou égale à Value. |
| IsWithin | `1` | La valeur de Field est comprise dans Value. |
| IsNotWithin | `9` | La valeur de Field n'est pas comprise dans Value. |
| Contains | `8` | La valeur de Field contient Value. |
| DoesNotContain | `10` | La valeur de Field ne contient pas Value. |
| ContainsExactly | `11` | La valeur de Field contient exactement Value. |
| IsOneOf | `12` | La valeur de Field est égale à l'une des valeurs spécifiées. Utilisé dans les AutoFilters. |
| Undefined | `0` | Valeur indéfinie. |
| IsAnyValue | `255` | Condition 'Is any value'. Applicable aux indicateurs graphiques. |

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


