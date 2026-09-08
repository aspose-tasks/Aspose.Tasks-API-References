---
title: "Tsk.IsRecurring"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, является ли задача частью серии повторяющихся задач"
type: docs
weight: 670
url: /ru/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Определяет, является ли задача частью серии повторяющихся задач.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


