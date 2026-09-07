---
title: "Tsk.StartVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo che rappresenta la differenza tra la data di inizio di base di un'attività o assegnazione e la sua data di inizio attualmente programmata."
type: docs
weight: 1040
url: /it/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

Il tempo che rappresenta la differenza tra la data di inizio di base di un'attività o assegnazione e la sua data di inizio attualmente programmata.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


