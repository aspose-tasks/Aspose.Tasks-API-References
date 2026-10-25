---
title: "Project.ResourceFilters"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene todas las definiciones de filtros basados en recursos. ResourceFilters es una colección de objetos Filter."
type: docs
weight: 760
url: /es/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Obtiene todas las definiciones de filtros basados en recursos. ResourceFilters es una colección de objetos [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## Ejemplos

Muestra cómo leer las definiciones de filtros de tareas/recursos.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Acceder a los filtros de recursos
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Ver también

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


