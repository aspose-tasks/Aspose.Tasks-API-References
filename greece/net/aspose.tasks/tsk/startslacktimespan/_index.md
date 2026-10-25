---
title: "Tsk.StartSlackTimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η διάρκεια μεταξύ των ημερομηνιών Έγκαιρης Έναρξης και Καθυστερημένης Έναρξης"
type: docs
weight: 1020
url: /el/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

Η διάρκεια μεταξύ των ημερομηνιών Έναρξη νωρίς και Έναρξη αργά.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε την ιδιότητα Tsk.StartSlackTimeSpan. Η ιδιότητα υπολογίζεται, έτσι συνήθως δεν χρειάζεται να τη ρυθμίσετε ρητά.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


