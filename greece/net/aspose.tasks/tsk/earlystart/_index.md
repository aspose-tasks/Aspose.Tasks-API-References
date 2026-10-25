---
title: "Tsk.EarlyStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η πιο πρώιμη ημερομηνία που μια εργασία μπορεί ενδεχομένως να ξεκινήσει, βάσει των πρώιμων ημερομηνιών έναρξης των προγενέστερων και επακόλουθων εργασιών και άλλων περιορισμών."
type: docs
weight: 340
url: /el/net/aspose.tasks/tsk/earlystart/
---
## Tsk.EarlyStart field

Η πιο πρώιμη ημερομηνία που μπορεί ενδεχομένως να ξεκινήσει μια εργασία, βάσει των πρώιμων ημερομηνιών έναρξης των προγενέστερων και επόμενων εργασιών και άλλων περιορισμών.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyStart;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.EarlyStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Start: " + task.Get(Tsk.EarlyStart));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


