---
title: "Tsk.WorkVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La differenza tra il lavoro di base di un'attività e il lavoro attualmente programmato"
type: docs
weight: 1160
url: /it/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

La differenza tra il lavoro di base di un'attività e il lavoro attualmente programmato.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


