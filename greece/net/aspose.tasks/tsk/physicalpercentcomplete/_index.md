---
title: "Tsk.PhysicalPercentComplete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Τιμή ποσοστού ολοκλήρωσης που μπορεί να χρησιμοποιηθεί ως εναλλακτική για τον υπολογισμό του προϋπολογισμένου κόστους εκτελεσθέντων εργασιών (BCWP)"
type: docs
weight: 900
url: /el/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Τιμή ποσοστού ολοκλήρωσης που μπορεί να χρησιμοποιηθεί ως εναλλακτική για τον υπολογισμό του προϋπολογισμένου κόστους εκτελεσθέντος έργου (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


