---
title: "Tsk.StartText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Επιστρέφει το κείμενο έναρξης της εργασίας"
type: docs
weight: 1030
url: /el/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Επιστρέφει το κείμενο έναρξης της εργασίας.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.StartText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


