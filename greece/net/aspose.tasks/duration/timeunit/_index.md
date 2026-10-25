---
title: "Duration.TimeUnit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Duration. Λαμβάνει τον τύπο μονάδας χρόνου για αυτό το αντικείμενο. Ο τύπος μονάδας χρόνου αυτής της παρουσίασης Duration."
type: docs
weight: 50
url: /el/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Λαμβάνει τον τύπο μονάδας χρόνου για αυτό το αντικείμενο. Ο τύπος μονάδας χρόνου της παρουσίας Duration.

```csharp
public TimeUnitType TimeUnit { get; }
```

## Παραδείγματα

Δείχνει πώς να ενημερώσετε μια διάρκεια εργασιών.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// λάβετε μια εργασία
var task1 = project.RootTask.Children.GetById(1);

// ενημερώστε τη διάρκεια της εργασίας
var duration1 = task1.Get(Tsk.Duration);

// προσθέστε μία ημέρα στην εργασία 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// ορίστε μια νέα διάρκεια στην εργασία
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// λάβετε μια άλλη εργασία
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// αλλάξτε τη διάρκεια χρησιμοποιώντας τον πραγματικό τύπο μονάδας χρόνου
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// ορίστε μια νέα διάρκεια στην εργασία
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Δείτε επίσης

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


