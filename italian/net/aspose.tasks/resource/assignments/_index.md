---
title: "Resource.Assignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Resource property. Ottiene una collezione di assegnazioni di risorse per questo oggetto"
type: docs
weight: 120
url: /it/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Ottiene una raccolta di assegnazioni di risorse per questo oggetto.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Esempi

Mostra come leggere le assegnazioni di una risorsa.

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

### Vedi anche

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


