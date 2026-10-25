---
title: "ResourceAssignment.ToString"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Возвращает краткое строковое представление экземпляра класса ResourceAssignment. Точные детали представления не указаны и могут измениться"
type: docs
weight: 790
url: /ru/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Возвращает краткое строковое представление экземпляра класса [`ResourceAssignment`](../). Точные детали представления не указаны и могут измениться.

```csharp
public override string ToString()
```

### Возвращаемое значение

краткая строка, представляющая объект назначения.

## Примеры

Показывает, как вывести общую информацию о назначении.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // отобразить назначения задачи
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


