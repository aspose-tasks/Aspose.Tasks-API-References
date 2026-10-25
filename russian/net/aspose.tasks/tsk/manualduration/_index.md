---
title: "Tsk.ManualDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет вручную запланированную длительность задачи"
type: docs
weight: 780
url: /ru/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Определяет вручную запланированную длительность задачи.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


