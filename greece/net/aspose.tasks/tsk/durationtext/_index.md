---
title: "Tsk.DurationText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Επιστρέφει το κείμενο διάρκειας της εργασίας"
type: docs
weight: 310
url: /el/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Επιστρέφει το κείμενο διάρκειας της εργασίας.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.DurationText.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


