---
title: "Tsk.ManualDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Definisce la durata pianificata manualmente di un'attività"
type: docs
weight: 780
url: /it/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Definisce la durata programmata manualmente di un'attività.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


