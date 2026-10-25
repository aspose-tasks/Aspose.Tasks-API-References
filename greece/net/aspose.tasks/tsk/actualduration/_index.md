---
title: "Tsk.ActualDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Η διάρκεια του πραγματικού χρόνου εργασίας για μια εργασία βάσει της προγραμματισμένης διάρκειας και της τρέχουσας εναπομείνας εργασίας ή του ποσοστού ολοκλήρωσης."
type: docs
weight: 30
url: /el/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

Η διάρκεια του πραγματικού χρόνου εργασίας για ένα έργο, βάσει του προγραμματισμένου διαστήματος και της τρέχουσας εναπομείνας εργασίας ή του ποσοστού ολοκλήρωσης.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις πραγματικές ιδιότητες της εργασίας.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


