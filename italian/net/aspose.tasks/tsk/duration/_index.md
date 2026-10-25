---
title: "Tsk.Duration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. L'intervallo totale di tempo di lavoro attivo per un'attività, inserito o calcolato da Microsoft Project in base alla data di inizio, data di fine, calendari e altri fattori di pianificazione."
type: docs
weight: 300
url: /it/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

L'intervallo totale di tempo di lavoro attivo per un'attività, inserito o calcolato da Microsoft Project in base alla data di inizio, data di fine, calendari e altri fattori di pianificazione.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Esempi

Mostra come impostare la durata dell'attività.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


