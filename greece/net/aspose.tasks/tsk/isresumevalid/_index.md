---
title: "Tsk.IsResumeValid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία μπορεί να συνεχιστεί"
type: docs
weight: 680
url: /el/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Καθορίζει εάν μια εργασία μπορεί να επανεκκινηθεί.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


