---
title: "Task.OutlineIndent"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Делает отступ задачи в структуре"
type: docs
weight: 1380
url: /ru/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Вставляет отступ для задачи в структуре.

```csharp
public void OutlineIndent()
```

## Примеры

Показывает, как сделать отступ задачи.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// отступить задачу
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


