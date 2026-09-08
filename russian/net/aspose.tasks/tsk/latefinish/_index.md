---
title: "Tsk.LateFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Последняя дата, когда задача может завершиться без задержки завершения проекта"
type: docs
weight: 730
url: /ru/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

Последняя дата, к которой задача может завершиться без задержки завершения проекта.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


