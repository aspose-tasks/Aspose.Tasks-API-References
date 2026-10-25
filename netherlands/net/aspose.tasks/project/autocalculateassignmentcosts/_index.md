---
title: "Project.AutoCalculateAssignmentCosts"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project eigenschap. Haalt op of stelt in of de toewijzingskosten en resterende kosten automatisch berekend moeten worden met behulp van de arbeid van toewijzingen en resource tarieven"
type: docs
weight: 70
url: /nl/net/aspose.tasks/project/autocalculateassignmentcosts/
---
## Project.AutoCalculateAssignmentCosts property

Haalt op of stelt in of de toewijzingskosten en resterende kosten automatisch moeten worden berekend met behulp van het werk van de toewijzing en de tarieven van de bron.

```csharp
public bool AutoCalculateAssignmentCosts { get; set; }
```

## Voorbeelden

Toont hoe de automatische berekening van toewijzingskosten uit te schakelen en de toewijzingskosten expliciet in te stellen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("New task");
task.Duration = project.GetDuration(TimeSpan.FromHours(15), TimeUnitType.Day);
var resource = project.Resources.Add("Resource");
resource.StandardRate = 10m;

var assignment = project.ResourceAssignments.Add(task, resource);

assignment.Work = project.GetDuration(TimeSpan.FromHours(12), TimeUnitType.Day);
assignment.ActualWork = project.GetDuration(TimeSpan.FromHours(3), TimeUnitType.Day);

Console.WriteLine("Now assignment's cost are auto calculated:");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);

project.AutoCalculateAssignmentCosts = false;
assignment.ActualCost = 123;
assignment.RemainingCost = 456;
assignment.Cost = 555;

Console.WriteLine("Now auto calculation of assignment's cost is turned off.");
Console.WriteLine("Actual Cost: {0}", assignment.ActualCost);
Console.WriteLine("Remaining Cost: {0}", assignment.RemainingCost);
Console.WriteLine("Cost: {0}", assignment.Cost);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


