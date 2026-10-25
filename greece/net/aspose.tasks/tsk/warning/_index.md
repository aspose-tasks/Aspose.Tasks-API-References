---
title: "Tsk.Warning"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Αντιπροσωπεύει τη σημαία που υποδεικνύει ότι η εργασία έχει αποκλίσεις στο χρονοδιάγραμμα"
type: docs
weight: 1120
url: /el/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Αντιπροσωπεύει τη σημαία που υποδεικνύει ότι η εργασία έχει αποκλίσεις στο χρονοδιάγραμμα.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε μια προειδοποίηση εργασίας.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


