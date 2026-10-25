---
title: "Enum FilterComparisonType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.FilterComparisonType enum. Il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per un filtro o indicatore grafico"
type: docs
weight: 620
url: /it/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Il tipo di confronto effettuato tra FieldName e Value che funge da criterio di selezione per un filtro o indicatore grafico.

```csharp
public enum FilterComparisonType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Equals | `6` | Il valore di Field è uguale a Value. |
| DoesNotEqual | `7` | Il valore di Field non è uguale a Value. |
| IsGreaterThan | `2` | Il valore di Field è maggiore di Value. |
| IsGreaterThanOrEqualTo | `4` | Il valore di Field è maggiore o uguale a Value. |
| IsLessThan | `3` | Il valore di Field è minore di Value. |
| IsLessThanOrEqualTo | `5` | Il valore di Field è minore o uguale a Value. |
| IsWithin | `1` | Il valore di Field è compreso in Value. |
| IsNotWithin | `9` | Il valore di Field non è compreso in Value. |
| Contains | `8` | Il valore di Field contiene Value. |
| DoesNotContain | `10` | Il valore di Field non contiene Value. |
| ContainsExactly | `11` | Il valore di Field contiene esattamente Value. |
| IsOneOf | `12` | Il valore di Field è uguale a uno dei Values specificati. Utilizzato negli AutoFilters. |
| Undefined | `0` | Valore non definito. |
| IsAnyValue | `255` | Condizione 'Is any value'. Applicabile agli indicatori grafici. |

## Esempi

Mostra come leggere i criteri del filtro attività.

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

// Stampa i criteri del filtro come stringa 
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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


