---
title: "Tsk.FinishText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Επιστρέφει το κείμενο λήξης της εργασίας"
type: docs
weight: 410
url: /el/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Επιστρέφει το κείμενο λήξης της εργασίας.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.FinishText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


