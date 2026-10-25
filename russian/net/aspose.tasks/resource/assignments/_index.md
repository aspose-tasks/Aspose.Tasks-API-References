---
title: "Resource.Assignments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает коллекцию назначений ресурсов для этого объекта"
type: docs
weight: 120
url: /ru/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Получает коллекцию назначений ресурсов для этого объекта.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Примеры

Показывает, как читать назначения ресурса.

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

### См. также

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


