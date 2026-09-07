---
title: "Tsk.IsSummary"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία είναι εργασία σύνοψης"
type: docs
weight: 720
url: /el/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Καθορίζει εάν μια εργασία είναι συνοπτική εργασία.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


