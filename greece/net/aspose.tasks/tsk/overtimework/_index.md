---
title: "Tsk.OvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το ποσό υπερωριών που έχει προγραμματιστεί να εκτελεστεί από όλους τους πόρους που έχουν ανατεθεί σε μια εργασία"
type: docs
weight: 870
url: /el/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

Το ποσό των υπερωριών που προγραμματίζονται να εκτελεστούν από όλους τους πόρους που έχουν ανατεθεί σε μια εργασία.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις υπερωρίες εργασιών.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Διαβάστε τις υπερωρίες και το ποσοστό ολοκλήρωσης για τις εργασίες
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Ορίστε το ποσοστό ολοκλήρωσης
    task.Set(Tsk.PercentComplete, 100);
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


