---
title: "AssignmentBaselineCollection.Count"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство AssignmentBaselineCollection. Получает количество объектов, содержащихся в этом объекте AssignmentBaselineCollection."
type: docs
weight: 10
url: /ru/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

Получает количество объектов, содержащихся в этом объекте AssignmentBaselineCollection.

```csharp
public int Count { get; }
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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


