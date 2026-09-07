---
title: "Tsk.ManualStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ορίζει την χειροκίνητα προγραμματισμένη έναρξη μιας εργασίας"
type: docs
weight: 800
url: /el/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Ορίζει την χειροκίνητα προγραμματισμένη έναρξη μιας εργασίας.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


