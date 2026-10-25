---
title: "Duration.TimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Duration. Λαμβάνει την παρουσία TimeSpan αυτού του αντικειμένου Duration. Η παρουσία TimeSpan αυτού του αντικειμένου Duration"
type: docs
weight: 40
url: /el/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Λαμβάνει την παρουσία `TimeSpan` αυτού του αντικειμένου Duration. Η παρουσία TimeSpan αυτού του αντικειμένου Duration.

```csharp
public TimeSpan TimeSpan { get; }
```

## Παραδείγματα

Δείχνει πώς να μετατρέψετε μια διάρκεια σε χρονικό διάστημα.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// λάβετε τη διάρκεια της εργασίας
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


