---
title: "Clase Filter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Filter. Representa un filtro en Project"
type: docs
weight: 600
url: /es/net/aspose.tasks/filter/
---
## Filter class

Representa un filtro en Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Filter](filter/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Obtiene o establece los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Obtiene el tipo del filtro. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Obtiene el índice de un objeto `Filter` en el objeto que contiene los Filters. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Obtiene o establece el nombre de un objeto Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Obtiene o establece un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filter en la pestaña Vista de la cinta de opciones. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Obtiene o establece un valor que indica si se muestran filas de resumen relacionadas para el filtro. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Obtiene el identificador único de un filtro. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Compara esta instancia con la instancia especificada de la clase `Filter` y devuelve una indicación de su orden relativo. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Devuelve un valor de código hash para el filtro. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Devuelve un valor que indica si esta instancia es mayor que un objeto especificado. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Devuelve un valor que indica si esta instancia es menor que un objeto especificado. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado. |

## Ejemplos

Muestra cómo trabajar con filtros.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// verificar filtros de recursos
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


