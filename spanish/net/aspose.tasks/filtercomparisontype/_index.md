---
title: "Enum FilterComparisonType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.FilterComparisonType enum. El tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para un filtro o indicador gráfico"
type: docs
weight: 620
url: /es/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

El tipo de comparación realizada entre FieldName y Value que actúa como criterio de selección para un filtro o indicador gráfico.

```csharp
public enum FilterComparisonType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Equals | `6` | El valor de Field es igual a Value. |
| DoesNotEqual | `7` | El valor de Field no es igual a Value. |
| IsGreaterThan | `2` | El valor de Field es mayor que Value. |
| IsGreaterThanOrEqualTo | `4` | El valor de Field es mayor que o igual a Value. |
| IsLessThan | `3` | El valor de Field es menor que Value. |
| IsLessThanOrEqualTo | `5` | El valor de Field es menor que o igual a Value. |
| IsWithin | `1` | El valor de Field está dentro de Value. |
| IsNotWithin | `9` | El valor de Field no está dentro de Value. |
| Contains | `8` | El valor de Field contiene Value. |
| DoesNotContain | `10` | El valor de Field no contiene Value. |
| ContainsExactly | `11` | El valor de Field contiene exactamente Value. |
| IsOneOf | `12` | El valor de Field es igual a uno de los Values especificados. Utilizado en AutoFilters. |
| Undefined | `0` | Valor indefinido. |
| IsAnyValue | `255` | Condición 'Is any value'. Aplicable a indicadores gráficos. |

## Ejemplos

Muestra cómo leer los criterios de filtro de tareas.

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

// criterios de filtro de impresión como una cadena 
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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


