---
title: "Tsk.IgnoreWarnings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Υποδεικνύει εάν πρέπει να κρύψετε το δείκτη προειδοποίησης σύγκρουσης προγράμματος στο Microsoft Project"
type: docs
weight: 540
url: /el/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Δείχνει εάν θα κρυφτεί η ένδειξη προειδοποίησης σύγκρουσης προγράμματος στο Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


