---
title: "Tsk.PreleveledFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата завершения задачи, как она была до выполнения выравнивания ресурсов"
type: docs
weight: 910
url: /ru/net/aspose.tasks/tsk/preleveledfinish/
---
## Tsk.PreleveledFinish field

Дата завершения задачи до выполнения выравнивания ресурсов.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledFinish;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.PreleveledFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Finish: " + task.Get(Tsk.PreleveledFinish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


