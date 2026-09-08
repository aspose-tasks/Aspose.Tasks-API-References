---
title: "Tsk.RemainingDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, необходимое для завершения незавершённой части задачи"
type: docs
weight: 960
url: /ru/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

Время, необходимое для завершения незавершённой части задачи.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


