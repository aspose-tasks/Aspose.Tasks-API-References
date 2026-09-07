---
title: "Tsk.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η τρέχουσα κατάσταση μιας εργασίας εκφρασμένη ως ποσοστό του έργου που έχει ολοκληρωθεί"
type: docs
weight: 890
url: /el/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

Η τρέχουσα κατάσταση μιας εργασίας εκφρασμένη ως ποσοστό του έργου που έχει ολοκληρωθεί.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


