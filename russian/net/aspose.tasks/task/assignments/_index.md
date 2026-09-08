---
title: "Task.Assignments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает коллекцию назначений ресурсов для этого объекта."
type: docs
weight: 120
url: /ru/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Получает коллекцию назначений ресурсов для этого объекта.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Примеры

Показывает, как перебрать назначения задачи.

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

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


