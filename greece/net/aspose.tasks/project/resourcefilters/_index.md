---
title: "Project.ResourceFilters"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει όλους τους ορισμούς φίλτρων βάσει πόρων. Το ResourceFilters είναι μια συλλογή αντικειμένων Filter."
type: docs
weight: 760
url: /el/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Λαμβάνει όλους τους ορισμούς φίλτρων βάσει πόρων. Το ResourceFilters είναι μια συλλογή αντικειμένων [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους ορισμούς φίλτρων εργασίας/πόρων.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Πρόσβαση σε φίλτρα πόρων
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Δείτε επίσης

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


