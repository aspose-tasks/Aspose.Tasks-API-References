---
title: "Resource.Assignments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Bu nesne için kaynak atamalarının bir koleksiyonunu alır"
type: docs
weight: 120
url: /tr/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Bu nesne için kaynak atamalarının bir koleksiyonunu alır.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Örnekler

Bir kaynağın atamalarının nasıl okunacağını gösterir.

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

### Ayrıca Bakınız

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


