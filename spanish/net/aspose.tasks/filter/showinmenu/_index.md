---
title: "Filter.ShowInMenu"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Filter. Obtiene o establece un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable de Filtros en la pestaña Vista de la cinta."
type: docs
weight: 60
url: /es/net/aspose.tasks/filter/showinmenu/
---
## Filter.ShowInMenu property

Obtiene o establece un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filter en la pestaña Vista de la cinta de opciones.

```csharp
public bool ShowInMenu { get; set; }
```

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

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


