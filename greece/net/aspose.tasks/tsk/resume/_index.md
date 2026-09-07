---
title: "Tsk.Resume"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ημερομηνία που το υπόλοιπο μέρος μιας εργασίας προγραμματίζεται να επανέλθει μετά την καταχώρηση οποιασδήποτε προόδου"
type: docs
weight: 1000
url: /el/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

Η ημερομηνία που το υπόλοιπο μέρος μιας εργασίας προγραμματίζεται να επαναληφθεί μετά την έναρξη οποιασδήποτε προόδου.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
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


