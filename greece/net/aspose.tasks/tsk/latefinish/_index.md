---
title: "Tsk.LateFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Η πιο πρόσφατη ημερομηνία που μια εργασία μπορεί να ολοκληρωθεί χωρίς να καθυστερήσει την ολοκλήρωση του έργου"
type: docs
weight: 730
url: /el/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

Η τελευταία ημερομηνία που μια εργασία μπορεί να ολοκληρωθεί χωρίς να καθυστερήσει την ολοκλήρωση του έργου.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


