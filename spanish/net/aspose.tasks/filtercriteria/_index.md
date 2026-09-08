---
title: "Clase FilterCriteria"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.FilterCriteria. Define los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP"
type: docs
weight: 630
url: /es/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Define los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP.

```csharp
public class FilterCriteria
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Obtiene la lista de filas hijas de `FilterCriteria`. Si el filtro contiene más de una fila de criterio, entonces el efecto de un operador And es que los criterios de ambas filas deben cumplirse para que la tarea o recurso se muestre como resultado de este filtro. El efecto de un operador Or es que los criterios de una u otra fila deben cumplirse. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Obtiene o establece un [`Field`](./field/) para cambiar. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Obtiene o establece el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Obtiene o establece el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Obtiene los valores de objeto para comparar con el valor del campo especificado con FieldName. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Obtiene si el valor del lado derecho de FilterCriteria es una referencia a un campo, no un valor constante. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Establece el campo cuyo valor será comparado con el valor del campo especificado por FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Devuelve la representación en cadena de la instancia de la clase `FilterCriteria`. |

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


