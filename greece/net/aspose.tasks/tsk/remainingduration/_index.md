---
title: "Tsk.RemainingDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ο χρόνος που απαιτείται για την ολοκλήρωση του ατελούς μέρους μιας εργασίας."
type: docs
weight: 960
url: /el/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

Ο χρόνος που απαιτείται για την ολοκλήρωση του ατελούς μέρους μιας εργασίας.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


