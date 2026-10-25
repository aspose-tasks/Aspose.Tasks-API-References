---
title: "Tsk.Type"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ο τύπος μιας εργασίας"
type: docs
weight: 1100
url: /el/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Ο τύπος μιας εργασίας.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


