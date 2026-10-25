---
title: "Tsk.BCWS"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Τα συνολικά χρονοπρογραμματισμένα κόστη βάσης μέχρι την ημερομηνία κατάστασης ή την τρέχουσα ημερομηνία"
type: docs
weight: 130
url: /el/net/aspose.tasks/tsk/bcws/
---
## Tsk.BCWS field

Τα συσσωρευτικά χρονομετρικά βασικά κόστη μέχρι την ημερομηνία κατάστασης ή τη σημερινή ημερομηνία.

```csharp
public static readonly Key<double, TaskKey> BCWS;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις τιμές κόστους εργασίας.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


