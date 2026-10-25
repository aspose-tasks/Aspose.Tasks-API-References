---
title: "Project.RecalculateResourceFields"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projectmethode. Herberekent Id Start en Finish van resources."
type: docs
weight: 1160
url: /nl/net/aspose.tasks/project/recalculateresourcefields/
---
## Project.RecalculateResourceFields method

Herberekent Id, Start en Finish van resources.

```csharp
public void RecalculateResourceFields()
```

## Voorbeelden

Toont hoe algemene resourcevelden opnieuw te berekenen.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 26, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1d, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 3, 26, 17, 0, 0));

var resource1 = project.Resources.Add("Res1");
resource1.Set(Rsc.Id, 2);
resource1.Set(Rsc.Start, new DateTime(2020, 3, 26, 8, 0, 0));
resource1.Set(Rsc.Finish, new DateTime(2020, 3, 26, 17, 0, 0));
var resource2 = project.Resources.Add("Res2");
resource2.Set(Rsc.Id, 1);
resource2.Set(Rsc.Start, new DateTime(2020, 3, 26, 8, 0, 0));
resource2.Set(Rsc.Finish, new DateTime(2020, 3, 26, 17, 0, 0));

var resourceAssignment1 = project.ResourceAssignments.Add(task, resource1);
resourceAssignment1.Set(Asn.Start, new DateTime(2020, 3, 25, 8, 0, 0));
resourceAssignment1.Set(Asn.Finish, new DateTime(2020, 3, 27, 17, 0, 0));

var resourceAssignment2 = project.ResourceAssignments.Add(task, resource2);
resourceAssignment2.Set(Asn.Start, new DateTime(2020, 3, 24, 8, 0, 0));
resourceAssignment2.Set(Asn.Finish, new DateTime(2020, 3, 24, 17, 0, 0));

Console.WriteLine("Resource 1 Id (before): " + resource1.Get(Rsc.Id));
Console.WriteLine("Resource 1 Start (before): " + resource1.Get(Rsc.Start));
Console.WriteLine("Resource 1 Finish (before): " + resource1.Get(Rsc.Finish));
Console.WriteLine("Resource 2 Id (before): " + resource1.Get(Rsc.Id));
Console.WriteLine("Resource 2 Start (before): " + resource1.Get(Rsc.Start));
Console.WriteLine("Resource 2 Finish (before): " + resource1.Get(Rsc.Finish));

// Herberekent Id, Start en Finish van resources
project.RecalculateResourceFields();

Console.WriteLine("Resource 1 Id (after): " + resource1.Get(Rsc.Id));
Console.WriteLine("Resource 1 Start (after): " + resource1.Get(Rsc.Start));
Console.WriteLine("Resource 1 Finish (after): " + resource1.Get(Rsc.Finish));
Console.WriteLine("Resource 2 Id (after): " + resource2.Get(Rsc.Id));
Console.WriteLine("Resource 2 Start (after): " + resource2.Get(Rsc.Start));
Console.WriteLine("Resource 2 Finish (after): " + resource2.Get(Rsc.Finish));
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


