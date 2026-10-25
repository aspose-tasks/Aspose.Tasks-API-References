---
title: "Tsk.DurationVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Разница между базовой длительностью задачи и текущей оценкой общей длительности задачи"
type: docs
weight: 320
url: /ru/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

Разница между базовой продолжительностью задачи и общей продолжительностью (текущей оценкой) задачи.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


