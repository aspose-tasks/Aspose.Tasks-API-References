---
title: "Resource.Assignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει μια συλλογή από αναθέσεις πόρων για αυτό το αντικείμενο"
type: docs
weight: 120
url: /el/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Λαμβάνει μια συλλογή από αναθέσεις πόρων για αυτό το αντικείμενο.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις αναθέσεις ενός πόρου.

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

### Δείτε επίσης

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


