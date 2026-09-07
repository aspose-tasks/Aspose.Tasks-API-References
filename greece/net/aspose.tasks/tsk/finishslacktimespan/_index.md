---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διάρκεια μεταξύ των ημερομηνιών Έγκαιρης Ολοκλήρωσης και Καθυστερημένης Ολοκλήρωσης"
type: docs
weight: 400
url: /el/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

Η διάρκεια μεταξύ των ημερομηνιών Early Finish και Late Finish.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε την ιδιότητα Tsk.FinishSlackTimeSpan. Η ιδιότητα υπολογίζεται, επομένως συνήθως δεν χρειάζεται να τη ρυθμίσετε ρητά.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


