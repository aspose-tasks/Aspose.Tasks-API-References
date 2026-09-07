---
title: "Tsk.IsManual"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία προγραμματίζεται χειροκίνητα"
type: docs
weight: 610
url: /el/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Καθορίζει εάν μια εργασία είναι προγραμματισμένη χειροκίνητα.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


