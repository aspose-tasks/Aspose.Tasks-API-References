---
title: "Tsk.FinishVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Tsk campo. Il tempo che rappresenta la differenza tra la data di fine baseline di un'attività o assegnazione e la sua data di fine attuale"
type: docs
weight: 420
url: /it/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

Il tempo che rappresenta la differenza tra la data di fine di base di un'attività o assegnazione e la sua data di fine attuale.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


