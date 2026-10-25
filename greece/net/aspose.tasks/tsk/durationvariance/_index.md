---
title: "Tsk.DurationVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Η διαφορά μεταξύ της βασικής διάρκειας μιας εργασίας και της συνολικής τρέχουσας εκτίμησης διάρκειας μιας εργασίας."
type: docs
weight: 320
url: /el/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

Η διαφορά μεταξύ της αρχικής διάρκειας μιας εργασίας και της συνολικής διάρκειας (τρέχουσας εκτίμησης) μιας εργασίας.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


