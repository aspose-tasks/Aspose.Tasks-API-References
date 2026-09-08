---
title: "Task.ParentTask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает родительскую задачу"
type: docs
weight: 940
url: /ru/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Получает родительскую задачу задачи.

```csharp
public Task ParentTask { get; }
```

## Примеры

Показывает, как использовать родительскую задачу.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


