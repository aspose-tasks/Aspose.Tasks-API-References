---
title: "Tsk.BCWP"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Η αθροιστική τιμή του ποσοστού ολοκλήρωσης της εργασίας πολλαπλασιασμένη με τα χρονοπρογραμματισμένα βασικά κόστη."
type: docs
weight: 120
url: /el/net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

Η συσσωρευτική τιμή του ποσοστού ολοκλήρωσης του έργου πολλαπλασιασμένη με τα χρονομετρικά βασικά κόστη.

```csharp
public static readonly Key<double, TaskKey> BCWP;
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


