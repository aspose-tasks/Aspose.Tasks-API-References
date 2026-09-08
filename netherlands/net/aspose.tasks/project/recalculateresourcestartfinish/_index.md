---
title: "Project.RecalculateResourceStartFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Rekent de start- en eindtijd van resources opnieuw"
type: docs
weight: 1170
url: /nl/net/aspose.tasks/project/recalculateresourcestartfinish/
---
## Project.RecalculateResourceStartFinish method

Rekent de start- en eindtijd van resources opnieuw.

```csharp
public void RecalculateResourceStartFinish()
```

## Voorbeelden

Toont hoe de start-/einddatums van resources opnieuw te berekenen.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 26, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1d, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 3, 26, 17, 0, 0));

var resource = project.Resources.Add("Res1");
resource.Set(Rsc.Start, new DateTime(2020, 3, 26, 8, 0, 0));
resource.Set(Rsc.Finish, new DateTime(2020, 3, 26, 17, 0, 0));

var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 3, 25, 8, 0, 0));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 3, 27, 8, 0, 0));

Console.WriteLine("Resource Start (before): " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Finish (before): " + resource.Get(Rsc.Finish));

// Berekent de start- en einddatums van resources opnieuw
project.RecalculateResourceStartFinish();

Console.WriteLine("Resource Start (after): " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Finish (after): " + resource.Get(Rsc.Finish));
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


