---
title: "Tsk.ActualCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Κόστη που προκύπτουν για εργασία που έχει ήδη εκτελεστεί από τους πόρους στις εργασίες τους, μαζί με τυχόν άλλα καταγεγραμμένα κόστη που σχετίζονται με την εργασία"
type: docs
weight: 20
url: /el/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Κόστη που προκύπτουν για εργασία που έχει ήδη εκτελεστεί από πόρους στα έργα τους, μαζί με τυχόν άλλα καταγεγραμμένα κόστη που σχετίζονται με το έργο.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


