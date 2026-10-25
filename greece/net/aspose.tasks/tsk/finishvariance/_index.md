---
title: "Tsk.FinishVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ο χρόνος που αντιπροσωπεύει τη διαφορά μεταξύ της ημερομηνίας λήξης βάσης μιας εργασίας ή ανάθεσης και της τρέχουσας ημερομηνίας λήξης"
type: docs
weight: 420
url: /el/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

Ο χρόνος που αντιπροσωπεύει τη διαφορά μεταξύ της αρχικής ημερομηνίας λήξης μιας εργασίας ή ανάθεσης και της τρέχουσας ημερομηνίας λήξης της.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


