---
title: "Tsk.CV"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διαφορά μεταξύ του κόστους βάσης και του συνολικού κόστους για μια εργασία. Διακύμανση κόστους  Κόστος  Κόστος βάσης"
type: docs
weight: 260
url: /el/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

Η διαφορά μεταξύ του αρχικού κόστους και του συνολικού κόστους για μια εργασία. Cost Variance = Cost - Baseline Cost

```csharp
public static readonly Key<double, TaskKey> CV;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις τιμές κόστους εργασίας.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


