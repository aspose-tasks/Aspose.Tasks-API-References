---
title: "FilterCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método FilterCollection. Convierte una colección de filtros en una lista de objetos Filter"
type: docs
weight: 90
url: /es/net/aspose.tasks/filtercollection/tolist/
---
## FilterCollection.ToList method

Convierte una colección de filtros en una lista de objetos [`Filter`](../../filter/).

```csharp
public List<Filter> ToList()
```

### Valor devuelto

Lista genérica de objetos [`Filter`](../../filter/).

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


