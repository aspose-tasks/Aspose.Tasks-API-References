---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Ο χρόνος που μια εργασία μπορεί να καθυστερήσει χωρίς να καθυστερήσει οποιεσδήποτε επακόλουθες εργασίες."
type: docs
weight: 450
url: /el/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

Ο χρόνος που μια εργασία μπορεί να καθυστερήσει χωρίς να καθυστερήσει τις επόμενες εργασίες.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε την ιδιότητα Tsk.FreeSlackTimeSpan. Η ιδιότητα υπολογίζεται, οπότε συνήθως δεν χρειάζεται να τη θέσετε ρητά.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


