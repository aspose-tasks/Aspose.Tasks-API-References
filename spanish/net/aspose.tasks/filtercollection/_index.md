---
title: "Clase FilterCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.FilterCollection. Contiene una lista de objetos Filter. Implementa la interfaz ICollectionFilter"
type: docs
weight: 610
url: /es/net/aspose.tasks/filtercollection/
---
## FilterCollection class

Contiene una lista de objetos [`Filter`](../filter/) . Implementa la interfaz ICollection&lt;Filter&gt;.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Elimina la primera aparición de un objeto específico de esta colección. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Convierte una colección de filtros en una lista de objetos [`Filter`](../filter/). |

## Ejemplos

Muestra cómo trabajar con colecciones de filtros.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// iterar sobre filtros de tareas
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// iterar sobre filtros de recursos
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// limpiar los filtros del proyecto de otro
otherProject.TaskFilters.Clear();

// copiar filtros a otro proyecto
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// agregar filtro de tarea personalizado
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// eliminar todos los filtros
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### Ver también

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


