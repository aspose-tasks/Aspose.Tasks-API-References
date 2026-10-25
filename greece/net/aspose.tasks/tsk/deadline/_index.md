---
title: "Tsk.Deadline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Μία ημερομηνία-στόχος που υποδεικνύει πότε πρέπει να ολοκληρωθεί μια εργασία"
type: docs
weight: 270
url: /el/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Μία ημερομηνία στόχος που υποδεικνύει πότε πρέπει να ολοκληρωθεί μια εργασία.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


