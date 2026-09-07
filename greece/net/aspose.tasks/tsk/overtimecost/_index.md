---
title: "Tsk.OvertimeCost"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Το συνολικό κόστος υπερωριών για μια εργασία για έναν πόρο σε όλες τις ανατεθειμένες εργασίες ή για μια ανάθεση πόρου"
type: docs
weight: 860
url: /el/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

Το συνολικό κόστος υπερωριών για μια εργασία, για έναν πόρο σε όλες τις ανατεθειμένες εργασίες ή για μια ανάθεση πόρου.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


