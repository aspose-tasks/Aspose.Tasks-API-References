---
title: "Tsk.EarlyFinish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Η πιο πρώιμη ημερομηνία που μια εργασία μπορεί ενδεχομένως να ολοκληρωθεί, βάσει των ημερομηνιών πρώιμης ολοκλήρωσης των προγενέστερων και επακόλουθων εργασιών, άλλων περιορισμών και τυχόν καθυστέρησης εξισορρόπησης"
type: docs
weight: 330
url: /el/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

Η πιο πρώιμη ημερομηνία που μπορεί ενδεχομένως να ολοκληρωθεί μια εργασία, βάσει των πρώιμων ημερομηνιών λήξης των προγενέστερων και επόμενων εργασιών, άλλων περιορισμών και τυχόν καθυστέρησης εξισορρόπησης.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.EarlyFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


