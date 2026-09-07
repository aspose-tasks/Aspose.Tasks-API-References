---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Ο χρόνος που η ημερομηνία λήξης μιας εργασίας μπορεί να καθυστερήσει χωρίς να καθυστερήσει την ημερομηνία λήξης του έργου."
type: docs
weight: 1090
url: /el/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

Ο χρόνος που η ημερομηνία λήξης μιας εργασίας μπορεί να καθυστερήσει χωρίς να καθυστερήσει την ημερομηνία λήξης του έργου.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε την ιδιότητα Tsk.TotalSlackTimeSpan. Η ιδιότητα υπολογίζεται, οπότε συνήθως δεν χρειάζεται να τη θέσετε ρητά.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


