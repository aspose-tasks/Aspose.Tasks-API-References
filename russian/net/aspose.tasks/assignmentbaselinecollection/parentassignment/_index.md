---
title: "AssignmentBaselineCollection.ParentAssignment"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство AssignmentBaselineCollection. Получает родительский ResourceAssignment для этой коллекции."
type: docs
weight: 30
url: /ru/net/aspose.tasks/assignmentbaselinecollection/parentassignment/
---
## AssignmentBaselineCollection.ParentAssignment property

Получает родительский объект [`ResourceAssignment`](../../resourceassignment/) для этой коллекции.

```csharp
public ResourceAssignment ParentAssignment { get; }
```

## Примеры

Показывает, как читать базовые линии назначений.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// читать информацию о базовой линии назначения
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// удалить базовые линии назначений
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### См. также

* class [ResourceAssignment](../../resourceassignment/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


