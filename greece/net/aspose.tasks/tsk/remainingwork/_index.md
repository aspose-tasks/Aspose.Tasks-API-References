---
title: "Tsk.RemainingWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Ο χρόνος που απαιτείται ακόμη για την ολοκλήρωση μιας εργασίας ή ενός συνόλου εργασιών"
type: docs
weight: 990
url: /el/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

Ο χρόνος που απαιτείται ακόμη για την ολοκλήρωση μιας εργασίας ή συνόλου εργασιών.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


