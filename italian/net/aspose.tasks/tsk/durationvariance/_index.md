---
title: "Tsk.DurationVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La differenza tra la durata di base di un'attività e la stima della durata totale corrente di un'attività."
type: docs
weight: 320
url: /it/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

La differenza tra la durata di base di un'attività e la durata totale (stima attuale) di un'attività.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


