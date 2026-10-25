---
title: "Tsk.IsNull"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk πεδίο. Καθορίζει εάν μια εργασία είναι μηδενική εργασία"
type: docs
weight: 640
url: /el/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Καθορίζει εάν μια εργασία είναι μηδενική εργασία.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


