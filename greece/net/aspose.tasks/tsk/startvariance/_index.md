---
title: "Tsk.StartVariance"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Ο χρόνος που αντιπροσωπεύει τη διαφορά μεταξύ μιας βασικής ημερομηνίας έναρξης μιας εργασίας ή ανάθεσης και της τρέχουσας προγραμματισμένης ημερομηνίας έναρξης."
type: docs
weight: 1040
url: /el/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

Ο χρόνος που αντιπροσωπεύει τη διαφορά μεταξύ μιας βασικής ημερομηνίας έναρξης μιας εργασίας ή ανάθεσης και της τρέχουσας προγραμματισμένης ημερομηνίας έναρξης.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


