---
title: "Tsk.ManualFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ορίζει το χειροκίνητα προγραμματισμένο τέλος μιας εργασίας"
type: docs
weight: 790
url: /el/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Ορίζει το χειροκίνητα προγραμματισμένο τέλος μιας εργασίας.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


