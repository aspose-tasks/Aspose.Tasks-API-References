---
title: "Tsk.IsExpanded"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Καθορίζει εάν μια εργασία σύνοψης είναι επεκτεταμένη ή όχι στην προβολή GanttChart"
type: docs
weight: 590
url: /el/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Καθορίζει εάν μια συνοπτική εργασία είναι επεκτεταμένη ή όχι στην προβολή GanttChart.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


