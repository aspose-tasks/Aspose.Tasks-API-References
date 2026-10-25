---
title: "Resource.Assignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-eigenschap. Haalt een verzameling van resource-toewijzingen op voor dit object"
type: docs
weight: 120
url: /nl/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Haalt een verzameling van resource-toewijzingen op voor dit object.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Voorbeelden

Toont hoe toewijzingen van een resource gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### Zie ook

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


