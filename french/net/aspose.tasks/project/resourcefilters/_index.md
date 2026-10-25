---
title: "Project.ResourceFilters"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient toutes les définitions de filtres basées sur les ressources. ResourceFilters est une collection d'objets Filter."
type: docs
weight: 760
url: /fr/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Obtient toutes les définitions de filtres basés sur les ressources. ResourceFilters est une collection d'objets [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## Exemples

Montre comment lire les définitions de filtres tâche/ressource.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Accéder aux filtres de ressources
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Voir aussi

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


