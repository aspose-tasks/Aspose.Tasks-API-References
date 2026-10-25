---
title: "Tsk.ActualWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το ποσό εργασίας που έχει ήδη ολοκληρωθεί από τους πόρους που έχουν εκχωρηθεί σε εργασίες"
type: docs
weight: 90
url: /el/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

Το ποσό εργασίας που έχει ήδη ολοκληρωθεί από τους πόρους που έχουν ανατεθεί σε έργα.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


