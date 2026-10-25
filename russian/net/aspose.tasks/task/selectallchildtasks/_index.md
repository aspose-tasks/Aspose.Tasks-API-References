---
title: "Task.SelectAllChildTasks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Рекурсивно собирает все дочерние задачи этой задачи"
type: docs
weight: 1400
url: /ru/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Рекурсивно собирает все дочерние задачи этой задачи.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Возвращаемое значение

Список дочерних задач этой задачи.

## Примеры

Показывает, как перебрать дочерние задачи.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


