---
title: "Task.Clone"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Создает полную копию задачи без подзадач"
type: docs
weight: 1310
url: /ru/net/aspose.tasks/task/clone/
---
## Task.Clone method

Создает полную копию задачи без подзадач.

```csharp
public object Clone()
```

### Возвращаемое значение

Создана копия задачи.

## Примеры

Показывает, как клонировать задачу.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


