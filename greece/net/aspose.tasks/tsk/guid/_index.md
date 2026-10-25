---
title: "Tsk.Guid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Οι παραγόμενοι μοναδικοί κωδικοί ταυτοποίησης για μια εργασία"
type: docs
weight: 460
url: /el/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

Οι παραγόμενοι μοναδικοί κωδικοί αναγνώρισης για μια εργασία.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


