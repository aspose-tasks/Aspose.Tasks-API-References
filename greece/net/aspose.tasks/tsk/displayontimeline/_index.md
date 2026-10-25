---
title: "Tsk.DisplayOnTimeline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία πρέπει να εμφανίζεται σε προβολή χρονοδιαγράμματος"
type: docs
weight: 290
url: /el/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Καθορίζει εάν μια εργασία πρέπει να εμφανίζεται σε προβολή χρονοδιαγράμματος.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


