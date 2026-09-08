---
title: "Task.Delete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Удаляет задачу из коллекции задач родительского проекта и все её назначения"
type: docs
weight: 1320
url: /ru/net/aspose.tasks/task/delete/
---
## Task.Delete method

Удаляет задачу из коллекции задач родительского проекта и все её назначения.

```csharp
public void Delete()
```

## Примеры

Показывает, как удалить задачу.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// удалить задачу
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


