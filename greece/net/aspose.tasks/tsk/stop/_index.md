---
title: "Tsk.Stop"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Η ημερομηνία που αντιπροσωπεύει το τέλος του πραγματικού μέρους μιας εργασίας"
type: docs
weight: 1060
url: /el/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

Η ημερομηνία που αντιπροσωπεύει το τέλος του πραγματικού τμήματος μιας εργασίας.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ημερομηνίες Stop/Resume της εργασίας.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Ελέγξτε τις ημερομηνίες Stop και Resume για όλες τις εργασίες
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


