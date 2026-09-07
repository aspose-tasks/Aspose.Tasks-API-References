---
title: "Tsk.StatusManager"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το όνομα του εταιρικού πόρου που θα λαμβάνει ενημερώσεις κατάστασης για την τρέχουσα εργασία από τους πόρους"
type: docs
weight: 1050
url: /el/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

Το όνομα του εταιρικού πόρου που θα λαμβάνει ενημερώσεις κατάστασης για την τρέχουσα εργασία από τους πόρους.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


