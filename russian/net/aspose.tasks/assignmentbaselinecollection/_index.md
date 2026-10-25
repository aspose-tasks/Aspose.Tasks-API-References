---
title: "Класс AssignmentBaselineCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.AssignmentBaselineCollection. Представляет коллекцию объектов AssignmentBaseline"
type: docs
weight: 60
url: /ru/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Представляет коллекцию объектов [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте AssignmentBaselineCollection. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Получает родительский [`ResourceAssignment`](../resourceassignment/) для этой коллекции. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Удаляет базовую линию из этой коллекции. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Преобразует объект AssignmentBaselineCollection в список объектов [`AssignmentBaseline`](../assignmentbaseline/). |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


