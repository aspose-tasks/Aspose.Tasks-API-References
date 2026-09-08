---
title: "Enum FilterComparisonType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.FilterComparisonType enum. Het type vergelijking dat wordt gemaakt tussen FieldName en Value en dient als selectiecriteria voor een filter of grafische indicator."
type: docs
weight: 620
url: /nl/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Het type vergelijking tussen FieldName en Value dat dient als selectiecategorie voor een filter of grafische indicator.

```csharp
public enum FilterComparisonType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Equals | `6` | De waarde van Field is gelijk aan Value. |
| DoesNotEqual | `7` | De waarde van Field is niet gelijk aan Value. |
| IsGreaterThan | `2` | De waarde van Field is groter dan Value. |
| IsGreaterThanOrEqualTo | `4` | De waarde van Field is groter dan of gelijk aan Value. |
| IsLessThan | `3` | De waarde van Field is kleiner dan Value. |
| IsLessThanOrEqualTo | `5` | De waarde van Field is kleiner dan of gelijk aan Value. |
| IsWithin | `1` | De waarde van Field ligt binnen Value. |
| IsNotWithin | `9` | De waarde van Field ligt niet binnen Value. |
| Contains | `8` | De waarde van Field bevat Value. |
| DoesNotContain | `10` | De waarde van Field bevat Value niet. |
| ContainsExactly | `11` | De waarde van Field bevat Value exact. |
| IsOneOf | `12` | De waarde van Field is gelijk aan een van de opgegeven Values. Wordt gebruikt in AutoFilters. |
| Undefined | `0` | Ongedefinieerde waarde. |
| IsAnyValue | `255` | 'Is any value'-conditie. Van toepassing op grafische indicatoren. |

## Voorbeelden

Toont hoe taakfiltercriteria te lezen.

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

// printfiltercriteria als een tekenreeks 
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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


