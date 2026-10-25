---
title: "Tsk.LateStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Η πιο πρόσφατη ημερομηνία που μια εργασία μπορεί να ξεκινήσει χωρίς να καθυστερήσει την ολοκλήρωση του έργου"
type: docs
weight: 740
url: /el/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

Η τελευταία ημερομηνία που μια εργασία μπορεί να ξεκινήσει χωρίς να καθυστερήσει την ολοκλήρωση του έργου.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


