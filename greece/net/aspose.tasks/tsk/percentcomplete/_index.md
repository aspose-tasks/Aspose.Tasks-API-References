---
title: "Tsk.PercentComplete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η τρέχουσα κατάσταση μιας εργασίας εκφρασμένη ως το ποσοστό της διάρκειας της εργασίας που έχει ολοκληρωθεί"
type: docs
weight: 880
url: /el/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

Η τρέχουσα κατάσταση μιας εργασίας, εκφρασμένη ως ποσοστό της διάρκειας της εργασίας που έχει ολοκληρωθεί.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Παραδείγματα

Δείχνει πώς να αλλάξετε την πρόοδο μιας εργασίας ενημερώνοντας το ποσοστό ολοκλήρωσης της εργασίας.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Πρόσβαση σε εργασίες και εμφάνιση του ποσοστού ολοκλήρωσης
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


