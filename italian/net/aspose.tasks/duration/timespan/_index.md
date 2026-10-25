---
title: "Duration.TimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Duration. Ottiene l'istanza TimeSpan di questo oggetto Duration. L'istanza TimeSpan di questo oggetto Duration"
type: docs
weight: 40
url: /it/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Ottiene l'istanza `TimeSpan` di questo oggetto Duration. L'istanza TimeSpan di questo oggetto Duration.

```csharp
public TimeSpan TimeSpan { get; }
```

## Esempi

Mostra come convertire una durata in un intervallo di tempo.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// ottieni la durata dell'attività
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


