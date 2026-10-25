---
title: "Tsk.WorkVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διαφορά μεταξύ της βασικής εργασίας μιας εργασίας και της τρέχουσας προγραμματισμένης εργασίας"
type: docs
weight: 1160
url: /el/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

Η διαφορά μεταξύ της βασικής εργασίας μιας εργασίας και της τρέχουσας προγραμματισμένης εργασίας.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


