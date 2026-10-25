---
title: "Tsk.IsSubproject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία είναι ένα ενσωματωμένο έργο"
type: docs
weight: 700
url: /el/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Καθορίζει εάν μια εργασία είναι ένα ενσωματωμένο έργο.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


