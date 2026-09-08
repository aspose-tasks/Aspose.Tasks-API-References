---
title: "ResourceAssignment.Baselines"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceAssignment. Возвращает объект AssignmentBaselineCollection. Коллекция значений базовых линий, связанных с назначением"
type: docs
weight: 120
url: /ru/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Получает объект AssignmentBaselineCollection. Коллекция базовых значений, связанных с назначением.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Примеры

Показывает, как получить доступ к базовым линиям назначения.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### См. также

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


