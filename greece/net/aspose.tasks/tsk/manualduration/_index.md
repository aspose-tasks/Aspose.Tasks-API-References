---
title: "Tsk.ManualDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ορίζει τη χειροκίνητα προγραμματισμένη διάρκεια μιας εργασίας"
type: docs
weight: 780
url: /el/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Ορίζει τη χειροκίνητα προγραμματισμένη διάρκεια μιας εργασίας.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


