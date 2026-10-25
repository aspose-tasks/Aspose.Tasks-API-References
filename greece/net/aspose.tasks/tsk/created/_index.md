---
title: "Tsk.Created"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ημερομηνία δημιουργίας μιας εργασίας"
type: docs
weight: 250
url: /el/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

Η ημερομηνία κατά την οποία δημιουργήθηκε μια εργασία.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


