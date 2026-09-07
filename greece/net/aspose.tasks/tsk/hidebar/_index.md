---
title: "Tsk.HideBar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν η μπάρα Gantt μιας εργασίας είναι κρυφή όταν εμφανίζεται στο Microsoft Project."
type: docs
weight: 480
url: /el/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Καθορίζει εάν η μπάρα Gantt μιας εργασίας είναι κρυφή όταν εμφανίζεται στο Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


