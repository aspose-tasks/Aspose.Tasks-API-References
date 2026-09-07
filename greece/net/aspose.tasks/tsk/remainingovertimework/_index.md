---
title: "Tsk.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η ποσότητα του εναπομείναντος προγραμματισμένου υπερωριακού χρόνου."
type: docs
weight: 980
url: /el/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

Το ποσό του υπολοίπου προγραμματισμένου χρόνου υπερωριών.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


