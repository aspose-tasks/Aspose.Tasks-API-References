---
title: "Task.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Возвращает значение хеш-кода для этой задачи."
type: docs
weight: 1350
url: /ru/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Возвращает значение хеш‑кода для этой задачи.

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш-код задачи.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// Хеш-код задачи основан на UID и имени задачи
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


