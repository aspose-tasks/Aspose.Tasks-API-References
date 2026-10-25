---
title: "Duration.TimeSpan"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-eigenschap. Haalt de TimeSpan‑instantie op van dit Duration‑object. De TimeSpan‑instantie van dit Duration‑object"
type: docs
weight: 40
url: /nl/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Haalt de `TimeSpan`‑instantie op van dit Duration‑object. De TimeSpan‑instantie van dit Duration‑object.

```csharp
public TimeSpan TimeSpan { get; }
```

## Voorbeelden

Toont hoe je een duur naar een time span kunt converteren.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// haal de taakduur op
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


