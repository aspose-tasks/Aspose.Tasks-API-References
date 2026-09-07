---
title: "Tsk.RemainingDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il tempo necessario per completare la parte non finita di un'attività"
type: docs
weight: 960
url: /it/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

Il tempo necessario per completare la parte non terminata di un'attività.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


