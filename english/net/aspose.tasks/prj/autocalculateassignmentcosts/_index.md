---
title: AutoCalculateAssignmentCosts
second_title: Aspose.Tasks for .NET API Reference
description: Determines whether assignment cost and remaining cost should be auto calculated using assignments work and resource rates.
type: docs
weight: 60
url: /net/aspose.tasks/prj/autocalculateassignmentcosts/
---
## Prj.AutoCalculateAssignmentCosts field

Determines whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

```csharp
public static readonly Key<bool, PrjKey> AutoCalculateAssignmentCosts;
```

### Examples

Shows how to turn of auto calculation of assignment's costs and to set assignment's costs explicitly.

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

### See Also

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [PrjKey](../../prjkey)
* class [Prj](../../prj)
* namespace [Aspose.Tasks](../../prj)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->