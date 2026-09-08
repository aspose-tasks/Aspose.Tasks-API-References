---
title: "Tsk.FinishVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, представляющее разницу между базовой датой завершения задачи или назначения и её текущей датой завершения"
type: docs
weight: 420
url: /ru/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

Время, представляющее разницу между базовой датой завершения задачи или назначения и её текущей датой завершения.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


