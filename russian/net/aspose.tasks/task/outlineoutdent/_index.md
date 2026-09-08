---
title: "Task.OutlineOutdent"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Перемещает задачу вверх в структуре"
type: docs
weight: 1390
url: /ru/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Поднимает задачу в структуре.

```csharp
public void OutlineOutdent()
```

## Примеры

Показывает, как уменьшить отступ задачи.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// уменьшить отступ задачи
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


