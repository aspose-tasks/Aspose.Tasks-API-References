---
title: "Tsk.PreleveledStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата начала задачи, как она была до выполнения выравнивания ресурсов"
type: docs
weight: 920
url: /ru/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

Дата начала задачи до выполнения выравнивания ресурсов.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.PreleveledStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


