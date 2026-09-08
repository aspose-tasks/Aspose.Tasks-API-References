---
title: "Tsk.IgnoreWarnings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Указывает, следует ли скрывать индикатор предупреждения о конфликте расписания в Microsoft Project"
type: docs
weight: 540
url: /ru/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Указывает, скрывать ли индикатор предупреждения о конфликте расписания в Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


