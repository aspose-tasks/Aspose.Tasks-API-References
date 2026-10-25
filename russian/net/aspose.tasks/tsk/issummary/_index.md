---
title: "Tsk.IsSummary"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, является ли задача сводной"
type: docs
weight: 720
url: /ru/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Определяет, является ли задача сводной задачей.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


